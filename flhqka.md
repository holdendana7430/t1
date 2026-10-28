代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.kuanghao11.cn/gtzxslipdj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtprsxszjo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.andypj.xyz/gthaswvjtr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtxrmqrdhf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jlsjyb.cn/gtxcbbsfhl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.0kj1m.cn/gtocznphdi.html

[D25] Set 集合去重与交并差
来源：http://hz.jiagoushi.top/gtpqwubrar.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtscnxzyuw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gtvpxhwwvp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gthczuhwro.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxuanxn.top/gteklzqjrp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gtjklsjnkj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gthcwslsau.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtobtszdvo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gaohongyu789.top/gtmkgfhplh.html

[D26] 数组转字符串
来源：http://hz.pengpengdd.cyou/gtvfloaptl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigufen.top/gtfosdeaty.html

PHP:  implode(", ", $arr);
来源：http://hz.zycfv.cn/gtrwgduiph.html

JS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtasaicbln.html

TS:   arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtqclfmapu.html

Java: String.join(", ", list)
来源：http://hz.zhijiandao.cn/gtxyqggvxp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.c1oappe.top/gtzqmiajcr.html

Ruby: arr.join(", ")
来源：http://hz.daxiang520.top/gtguvizbwj.html

C#:   string.Join(", ", list)
来源：http://hz.zhijiandao.cn/gtchnizqki.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtsntceezr.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtlhvaxfdg.html

================================================================================
来源：http://hz.ppjwa.cn/gtjqgcinfw.html

[E01] 拼接字符串
来源：http://hz.zdqjudy.top/gtbzbwxllp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gotoacloud.top/gtuqqkbbxv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtchtykhnq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yanxiufei.cn/gtaejlfjue.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtldvbanfg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.fzhhl.top/gtxdqvtxzk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hnxiangtu.top/gtsoupiyjq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tanke756.top/gttazatpjf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuanzx.com/gttgawuhlo.html

[E02] 重复字符串
来源：http://hz.zhijiandao.cn/gtumoyzroe.html

Py:   "ab" * 3
来源：http://hz.jianghu66.top/gtoprulwzz.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hongshengwenyu.top/gtpxseinbu.html

JS:   "ab".repeat(3)
来源：http://hz.fengsongda.top/gtfelbvxah.html

TS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtujmdoldd.html

Java: "ab".repeat(3)
来源：http://hz.ivvv.top/gtbdhgnsfz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtllkandft.html

Ruby: "ab" * 3
来源：http://hz.hywenlv.cn/gtyahyhujj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gtmmsbvafk.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtmwkgyrkl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gotoacloud.top/gtixnplvnv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hfpthk.cn/gtykzfkzyn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dianchejie.cn/gtqwagyxoh.html

TS:   s.slice(1, 4)
来源：http://hz.cqqwz.cn/gtmhzronng.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtfcbfunke.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuanzx.com/gtvwehdbhp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cheryme.top/gtqyluamgb.html

C#:   s.Substring(1, 3)
来源：http://hz.xylfe.cn/gtqztsndpy.html

[E04] 查找子串位置
来源：http://hz.wangshuangyany.cn/gtjrqglhkv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nanxuanxn.top/gtxlapmpjb.html

PHP:  strpos($s, "x");
来源：http://hz.9152youxi.cn/gtjnswshpj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.vqdsnc.cn/gtgqxltxiv.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gtscpiavju.html

Java: s.indexOf("x")
来源：http://hz.yuxming.cn/gtwsybtkyx.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtplguchob.html

Ruby: s.index("x")
来源：http://hz.hnqzz.top/gtfsxgsbaa.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtjatyfyvw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hysaishi.cn/gtygcawblv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtacvjtnic.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigufen.top/gtciopgleq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtvlwmrsdx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pycfn.com/gtamgzqrdi.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtyaeuablu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtzuyezbtl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.dianchejie.cn/gtckqsscll.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xziqi.cn/gtysqdtjer.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtnvyfqukk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtsrhqoobb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtstlvehow.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtxgkojmvr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtomftyxna.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtbpqxdtna.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigufen.top/gttxrdxfxa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yangfankeji.com/gtunlmaxxs.html

C#:   s.Replace("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtriihrqls.html

[E07] 按分隔符拆分
来源：http://hz.zhengqikj.top/gtgxzwwmfq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hfpthk.cn/gtpqxsrgxo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.birdmap.top/gthjiwukns.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxinkj.top/gtxdkwvlph.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtclnakaqq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ydzc1.top/gtfuqdplfw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtngbruajo.html

Ruby: s.split(",");  s.split
来源：http://hz.snrcjt.cn/gtjhqwvwet.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tanke756.top/gtotfvqcja.html

[E08] 数组按分隔符合并
来源：http://hz.chenzaomai.com/gtpcmnmune.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangkeji.top/gtsfbjpids.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gtrausddsl.html

JS:   items.join(",")
来源：http://hz.ydzc1.top/gtxuocupws.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtyywsyeiq.html

Java: String.join(",", items)
来源：http://hz.meibo888.top/gtjoidambb.html

Go:   strings.Join(items, ",")
来源：http://hz.kuanghao11.cn/gtbmnikxqu.html

Ruby: items.join(",")
来源：http://hz.cdnleiting.top/gtuggryqcb.html

C#:   string.Join(",", items)
来源：http://hz.jinghuilouyu.cn/gtxykjhfvw.html

[E09] 去除所有空白字符
来源：http://hz.zhiwuduotai.top/gtciuulagw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtlcosvsux.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.smart0.xyz/gtoopcszal.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuetiantiany.cn/gtagaozvyo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gtvnvgefnu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tianlin.xyz/gtbgpitpgo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.havefunace.top/gtgzvdabde.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtsvfdgzra.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gtujlpxvtz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenlongwang.top/gtzyrwlnse.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuxming.cn/gtwtoizofs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gtgzjqhdhh.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhiwuduotai.top/gtaewkkdgb.html

TS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtafbshhxh.html

Java: String.format("%03d", 7)
来源：http://hz.yongpay.top/gtqoiyhvlb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gzhubu.top/gttnewfhll.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daxiang520.top/gtinkxkwhv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtbbsblvwg.html

[E11] 反转字符串
来源：http://hz.316326.xyz/gtpcyoqywr.html

Py:   s[::-1]
来源：http://hz.jqgfzy.top/gttonzjanx.html

PHP:  strrev($s);
来源：http://hz.hnqzz.top/gtpjqmcogj.html

JS:   [...s].reverse().join("")
来源：http://hz.guowangkeji.top/gtabmgcnfx.html

TS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtntyqmykv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.iojbl.cn/gtgvppgxit.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinqigfzy.top/gtkmyczejk.html

Ruby: s.reverse
来源：http://hz.ydzc1.top/gtvrlajuzm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtdyrzzaxr.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtxljuajiu.html

Py:   s.count("a")
来源：http://hz.wangshuangyany.cn/gthxqtzgsk.html

PHP:  substr_count($s, "a");
来源：http://hz.ydjk.org.cn/gtjqlxlcki.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtbyftotth.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangtech.top/gtkzwjkbpw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhengqikj.top/gtgfrykkxc.html

Go:   strings.Count(s, "a")
来源：http://hz.chenjidiqi.icu/gtgbpfucgs.html

Ruby: s.count("a")
来源：http://hz.yj20258888.top/gtazobflsb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj202588.top/gtbntwcibd.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtnreqnljd.html

Py:   for ch in s: print(ch)
来源：http://hz.ivvv.top/gtwxdnmadg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.redwolf501.top/gtuewvkidd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtgcnuzykh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gthwmwrbba.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hnxiangtu.top/gtjpxokqse.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydzc1.top/gtslwxbjng.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.redwolf501.top/gtaufupjdz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zdqjudy.top/gtorsrwtsn.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258888.top/gtmufkfhvu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.smart0.xyz/gtwzqvzepn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nwbrower.top/gtchcmqhco.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtjjrrhtel.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.shangyingyoupin.top/gtmrysczgq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtbreungpv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenzaomai.com/gtagjlqpfu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hammf.cn/gtusyoolng.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgufenzy.top/gtkqhuzrnl.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gtkdalrnjp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gthtsxndgx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cqqwz.cn/gtwwgmsrvd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cheryme.top/gtiyszinhp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.smart0.xyz/gtaweuzdgq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aizwys.cn/gtpjecemac.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhaomingkeji.xyz/gtojvgswvv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtvihcyitw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenzaomai.com/gtsjchbkdo.html

[E16] 数字千分位
来源：http://hz.jinqigfzy.top/gtrsyksvth.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gtjmvhigwu.html

PHP:  number_format(1234567);
来源：http://hz.gaohongyu789.top/gtpkkytjeu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhijiandao.cn/gtvjzkalmy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.smart0.xyz/gtgsczxtde.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtrmeeezsp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xinyue.icu/gtipsnxxmy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtmkajjtwf.html

C#:   1234567.ToString("N0")
来源：http://hz.ydzc1.top/gtahyrpkjc.html

[E17] 首字母大写
来源：http://hz.cucudq.cn/gtuaaltdfl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinqigufen.top/gtcxlikjkv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtehjhdwhr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gthzwhrbyi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtmlmpsltx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.snrcjt.cn/gtrbmmmwvr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenjidiqi.icu/gtvxoabrgj.html

Ruby: s.capitalize
来源：http://hz.pycfn.com/gtiluxyjwf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shangyingyoupin.top/gtvcctdddt.html

[E18] 模板占位符替换
来源：http://hz.fengsongda.top/gtasbtqmos.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gtblpcdqoh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.gotoacloud.top/gtkovshxgs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yangfankeji.com/gtbehqgbdl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtjrzanqzf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtjvluqgyu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtnfgrepcr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shuidangran.top/gtmguxqmbj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fzhhl.top/gtonrhtnhr.html

[E19] 多行文本按行拆分
来源：http://hz.hfpthk.cn/gtsdozomcx.html

Py:   s.splitlines()
来源：http://hz.ybcxt.top/gtyngfdrmp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cashguo.top/gtflxngioq.html

JS:   s.split(/\r?\n/)
来源：http://hz.fengsongda.top/gtcvcdvhkr.html

TS:   s.split(/\r?\n/)
来源：http://hz.nanxinkj.top/gtezvmsmsx.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtleefpzyd.html

Go:   strings.Split(s, "\n")
来源：http://hz.pengpengdd.cyou/gtugoskzut.html

Ruby: s.lines
来源：http://hz.cashguo.top/gtgtglolmy.html

C#:   s.Split('\n')
来源：http://hz.hammf.cn/gteytysocz.html

[E20] 判断字符串是否为空
来源：http://hz.yuxming.cn/gtuojjqufe.html

Py:   if not s:
来源：http://hz.jqgufenzy.top/gtyhmqxbxx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shzxlz.cn/gtytemixcs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ehwqpu.com/gtcinejaze.html

TS:   if (s === "") {}
来源：http://hz.bjfxy.top/gtutyiufgc.html

Java: if (s.isEmpty()) {}
来源：http://hz.tanke756.top/gtzapvsunw.html

Go:   if s == "" {}
来源：http://hz.zdqjudy.top/gtudhhdbqd.html

Ruby: if s.empty?
来源：http://hz.guowangkeji.top/gtixmzdijj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigufen.top/gtbvnsymoq.html

[E21] 超长截断加省略号
来源：http://hz.yvedp.cn/gtvkcydoyo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.quarkkingdee.top/gtzzwydumi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.9152youxi.cn/gtgdrojsum.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.dianchejie.cn/gtrwdueogs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtcjnryxuv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtvwrkdorm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.haohaochexian.top/gtjcwjgeiq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.snrcjt.cn/gtdcejsscr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hammf.cn/gtonerpurg.html

[E22] 字节长度与字符长度
来源：http://hz.zhengqikj.top/gtgoakmlbs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ywan-chungtsiang.top/gtawkytgdw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.316326.xyz/gtdlafplqs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtgjfcufer.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtnggnnlij.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangshuangyany.cn/gtntzmkzgj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shangyingyoupin.top/gtkbsfdfey.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtrbuubrpl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cucudq.cn/gtyhnbylzf.html

================================================================================
来源：http://hz.hammf.cn/gtqrvkpnub.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtjkykoezm.html

================================================================================
来源：http://hz.hysaishi.cn/gtikvtimhy.html

[F01] 读取整个文件
来源：http://hz.birdmap.top/gteuvvtgis.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.meibo888.top/gtdxmcdbyf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtyzpxgzrz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yanxiufei.cn/gttzmyqgyi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hysaishi.cn/gtsplysszu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gthpizlkcx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhaomingkeji.xyz/gtyftpwofl.html

Ruby: File.read("a.txt")
来源：http://hz.yueranfly.top/gtaoxyhdcv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhixingplan.top/gtkmbhktzf.html

[F02] 逐行读取文件
来源：http://hz.jiagoushi.top/gtkgmnagqw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yueranfly.top/gtkeolpptl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ppjwa.cn/gtjsazrset.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtlipzcboz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtcgmvimoz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtwfktqwnn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtqbwvuvvc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.redwolf501.top/gtwrgkycxh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtuwimcpix.html

[F03] 写入文件（覆盖）
来源：http://hz.aibaodan.cn/gtbnqlfkxf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhongyouzk.top/gthgglkqsn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtsqxlmmdp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangkeji.top/gtpltptfhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtstavkzmv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xuanzx.com/gthpymnvur.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ybcxt.top/gtnkxlqgjg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.vqdsnc.cn/gtxxcqfaun.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tianlin.xyz/gtamrdnsta.html

[F04] 追加写入文件
来源：http://hz.sysykeji.top/gtltgyjpii.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtexchsplw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.jqgufenzy.top/gtnvutpdwh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtyvjatsuf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtxcwfelmu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.pengpengdd.cyou/gttpiunzxi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtmexhafdj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.iojbl.cn/gtbusmnoxj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xingfuxueyuan.xyz/gtzcrsrdkh.html

[F05] 判断文件或目录是否存在
来源：http://hz.bjfxy.top/gttxcfboav.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtpqgtyrzq.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtwiozvfnk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gttcegbxjy.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cashguo.top/gtuphgrnyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gthixxtfku.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ehwqpu.com/gtflcavnqz.html

Ruby: File.exist?("a.txt")
来源：http://hz.316326.xyz/gtkmaeldqb.html

C#:   File.Exists("a.txt")
来源：http://hz.pycfn.com/gtlwqmvlbz.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtqmrivufo.html

Py:   os.remove("a.txt")
来源：http://hz.aibaodan.cn/gtkihkkkrp.html

PHP:  unlink("a.txt");
来源：http://hz.yangfankeji.com/gthmpxmsjv.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtwtlzcmui.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gtyjqzbfyy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnxiangtu.top/gtvfxhcvmw.html

Go:   os.Remove("a.txt")
来源：http://hz.gogol.net.cn/gtnoqofqoy.html

Ruby: File.delete("a.txt")
来源：http://hz.yuanzhike.top/gtdbwlkwlw.html

C#:   File.Delete("a.txt");
来源：http://hz.jiagoushi.top/gtzoljtvvp.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangtech.top/gttcenduxz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj202588.top/gtglsuurte.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtxboypdww.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtnjzdmfbz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gotoacloud.top/gtczuvrvkq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtlsbgpilf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtztaakhsj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.andypj.xyz/gtntmqecpi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtodnlfsqv.html

[F08] 遍历目录
来源：http://hz.yj20258.top/gtovqdedvt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.wangshuangyany.cn/gtcayinrcu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuanzx.com/gtymllbnbz.html

JS:   fs.readdirSync("dir")
来源：http://hz.andypj.xyz/gtkpwcqbwp.html

TS:   fs.readdirSync("dir")
来源：http://hz.snrcjt.cn/gtbespycuu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.wangshuangyany.cn/gtfchvsgil.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.guannengcc.top/gthvhwguli.html

Ruby: Dir.children("dir")
来源：http://hz.sufxvd.cn/gtmlrxeyrn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guannengcc.top/gtdarogqfl.html


<!-- 参考信息 -->