代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.havefunace.top/gtilgivyzg.html

[D24] 字典 / Map 基本操作
来源：http://hz.9152youxi.cn/gtdtokxqcx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cqqwz.cn/gtzmpcjsgv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.vqdsnc.cn/gtljqowdpn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gtchmuzsca.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.316326.xyz/gtkombnmgc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhijiandao.cn/gteorerowb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sysykeji.top/gtkoieippt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guannengcc.top/gtpzwmixqd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shuidangran.top/gtaegrnuza.html

[D25] Set 集合去重与交并差
来源：http://hz.ydzc1.top/gtpbgkgyud.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj202588.top/gtcuciqskw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shanyushiyangtech.top/gtuevqvlob.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhijiandao.cn/gtyqccaeov.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtouidpslo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.kuanghao11.cn/gtpshadnrx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cqqwz.cn/gtazffeval.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigfzy.top/gtrjdukisp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.c1oappe.top/gtkjnnlofq.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtytxtkyci.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gtnpsolloa.html

PHP:  implode(", ", $arr);
来源：http://hz.guannengcc.top/gtmvffogmx.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtbtfparga.html

TS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtegfuqsbf.html

Java: String.join(", ", list)
来源：http://hz.xuetiantiany.cn/gtrgemvqyr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuxming.cn/gtzxnpxyqq.html

Ruby: arr.join(", ")
来源：http://hz.zhengqikj.top/gtxclelvut.html

C#:   string.Join(", ", list)
来源：http://hz.c1oappe.top/gtommuwpyx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtferaoyuk.html

E. 字符串处理
来源：http://hz.xinyue.icu/gtzlvskods.html

================================================================================
来源：http://hz.hnxiangtu.top/gtymwbbaqi.html

[E01] 拼接字符串
来源：http://hz.tian-w.cn/gtmyxrylbq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jyoumei.cn/gtwrutdtfp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.guowangkeji.top/gtfhmumrxz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gthhhyuhtx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gttunocwfc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenlongwang.top/gtlprjxeca.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cashguo.top/gthytqqfsz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hywenlv.cn/gtihdeazpy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtjhfasyhs.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtmaxespcw.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtgchbtuga.html

PHP:  str_repeat("ab", 3);
来源：http://hz.316326.xyz/gtwaaieugn.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtiamihxnx.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtbdbhfppk.html

Java: "ab".repeat(3)
来源：http://hz.gzhubu.top/gtjudxmcrn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtcemrgkhk.html

Ruby: "ab" * 3
来源：http://hz.ppjwa.cn/gtlmcvyqek.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gtxgisjcsv.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtxsqtqgnv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gthbiwapwv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fzhhl.top/gtmttecgpb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtglroowkv.html

TS:   s.slice(1, 4)
来源：http://hz.jqgfzy.top/gtkghuuhro.html

Java: s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtskrcqrzx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtxtfpctfl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ywan-chungtsiang.top/gtluywqgam.html

C#:   s.Substring(1, 3)
来源：http://hz.vqdsnc.cn/gtarlfbmbk.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gtkqsmvoxq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gzhubu.top/gtmxzoucfd.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtxzkcwfjz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ybcxt.top/gtsjmhcxbf.html

TS:   s.indexOf("x")
来源：http://hz.hnqzz.top/gtfihrfiji.html

Java: s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtcblgtdnd.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtouypieax.html

Ruby: s.index("x")
来源：http://hz.hfpthk.cn/gtiwxwsels.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtazsnevpc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtpcqnbpkt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtstimjwtl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.kuanghao11.cn/gtaemsaoie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gtviogehwg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gaohongyu789.top/gtjizsafxc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtifurqrug.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gttejyimmj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yonumen.top/gticlpuske.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sxryk.cn/gtbmaaozmy.html

[E06] 替换子串
来源：http://hz.zycfv.cn/gtucaaaemb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtewqywsad.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.9152youxi.cn/gtnpyihpue.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtzabbhsfi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhixingplan.top/gtlctyfoug.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtzxplzcvt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tian-w.cn/gtzjihvrmh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtszoptzgp.html

C#:   s.Replace("a", "b")
来源：http://hz.ydzc1.top/gtwnceelig.html

[E07] 按分隔符拆分
来源：http://hz.zhengqikj.top/gtzymdscvr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hywenlv.cn/gtzycamlte.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pycfn.com/gtdlcxihvl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydjk.org.cn/gtvqkliomr.html

TS:   s.split(",")
来源：http://hz.ivvv.top/gtpvhxdteo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yvedp.cn/gtwincnvab.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jianghu66.top/gtddlsrwhu.html

Ruby: s.split(",");  s.split
来源：http://hz.jqgfzy.top/gtadgptret.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.pengpengdd.cyou/gtbjgjuhjk.html

[E08] 数组按分隔符合并
来源：http://hz.yj202588.top/gtudgiapdo.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtvbmtaxli.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gtsaqhdrkd.html

JS:   items.join(",")
来源：http://hz.0kj1m.cn/gtmwnpksxe.html

TS:   items.join(",")
来源：http://hz.0kj1m.cn/gtslaeinar.html

Java: String.join(",", items)
来源：http://hz.zhongyouzk.top/gtdholsjvs.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gttplihczm.html

Ruby: items.join(",")
来源：http://hz.gogol.net.cn/gtrhonmmbn.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtlnoshmyb.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtkmsltbke.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.c1oappe.top/gtvgpuyjqq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shzxlz.cn/gtiajzgmuo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtontiqxol.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jqgufenzy.top/gtbjkyjkgo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gogol.net.cn/gtamhfmvmm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hywenlv.cn/gtsbfkyxec.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangshuangyany.cn/gtvatrufqi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gthaxitfzg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.mhx1999.top/gtldryfzil.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtqnkdjhyu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtcykgytye.html

JS:   "7".padStart(3, "0")
来源：http://hz.xinyue.icu/gtlicwisqu.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnxiangtu.top/gtjofcobmz.html

Java: String.format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtkxzffuuh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtpbfcrden.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yvedp.cn/gtulvfodhq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gzhubu.top/gtwwenvwhx.html

[E11] 反转字符串
来源：http://hz.cashguo.top/gtpaieaaje.html

Py:   s[::-1]
来源：http://hz.zhoulong.xyz/gtvdaoejvz.html

PHP:  strrev($s);
来源：http://hz.aibaodan.cn/gtfzzqtdyq.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtkdslseqh.html

TS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtiucuofhl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.svipenyu.cn/gtixvrrpeo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenzaomai.com/gtnyyiwznp.html

Ruby: s.reverse
来源：http://hz.havefunace.top/gtkydkevpg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtfvkobaut.html

[E12] 统计某字符出现次数
来源：http://hz.gzhubu.top/gtxyzvuwkh.html

Py:   s.count("a")
来源：http://hz.chenzaomai.com/gtmptblwqr.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtmonyslyl.html

JS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gttapqdmwu.html

TS:   s.split("a").length - 1
来源：http://hz.mhx1999.top/gteombuhxg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jqgufenzy.top/gtfbrjhxtb.html

Go:   strings.Count(s, "a")
来源：http://hz.quarkkingdee.top/gtwemgiwxa.html

Ruby: s.count("a")
来源：http://hz.fzhhl.top/gtggmmreis.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtdynibyrx.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtcsbwpaug.html

Py:   for ch in s: print(ch)
来源：http://hz.xinyue.icu/gtevjgydja.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuanzx.com/gtxnejjzpk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtellqcczq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtavakqqpo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtxsvbsynn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuanzx.com/gthxxwaxpj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtkxelsjop.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtrqzhpogo.html

[E14] URL 编码与 Base64
来源：http://hz.jyoumei.cn/gtrnfoncot.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhixingplan.top/gtyykoxkjm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ybcxt.top/gtrmiatelq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gtikdwiagw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.meibo888.top/gtelsvzpsp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ivvv.top/gtyqbibizf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuxming.cn/gtwspopaes.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtltbwckxt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.wangdashe.top/gtowwngyjn.html

[E15] HTML 转义 / 反转义
来源：http://hz.cashguo.top/gtyommwmfw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtoefpzejc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhongyouzk.top/gtmtdxiqom.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.mhx1999.top/gtuihmpfke.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj202588.top/gtuucqfndf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydjk.org.cn/gtzzszwltn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtnhfyxmtc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtwgqiumqc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jlsjyb.cn/gtceynjvzg.html

[E16] 数字千分位
来源：http://hz.316326.xyz/gtyivkbfcy.html

Py:   f"{1234567:,}"
来源：http://hz.xuanzx.com/gtdwkqyosg.html

PHP:  number_format(1234567);
来源：http://hz.tian-w.cn/gtnpvzklst.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangkeji.top/gtyaqnikhy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtqonhewpr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gtcglkpnkf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cqqwz.cn/gtandclggc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtrlbfsbke.html

C#:   1234567.ToString("N0")
来源：http://hz.jqgfzy.top/gtrbovvmri.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gtghbjdyrk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zdqjudy.top/gtfnbnulcw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.haohaochexian.top/gtmdfyaedd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtahzzmubo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.quarkkingdee.top/gtzpwvwggf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtydtejogu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtddtdsirv.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gthjwhicsc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yuanzhike.top/gtrpjzdffn.html

[E18] 模板占位符替换
来源：http://hz.wangdashe.top/gtvirmrsgp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.0kj1m.cn/gtfmjzkbat.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtpagliffg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtmwnhorzd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtftsgoifh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinqigufen.top/gtabefhuth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.316326.xyz/gtxilqgdta.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tianlin.xyz/gtmslxylqy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hammf.cn/gtsefglwcc.html

[E19] 多行文本按行拆分
来源：http://hz.cqqwz.cn/gtbhshumcm.html

Py:   s.splitlines()
来源：http://hz.dashuyun.cn/gttpvhghjk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.dashuyun.cn/gtuktfqfws.html

JS:   s.split(/\r?\n/)
来源：http://hz.daria6918.cn/gtwnmgfsum.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinghuilouyu.cn/gtxupadzjm.html

Java: s.lines().toList()
来源：http://hz.dianchejie.cn/gtcporhyue.html

Go:   strings.Split(s, "\n")
来源：http://hz.yonumen.top/gtniekavqx.html

Ruby: s.lines
来源：http://hz.jlsjyb.cn/gtniwudxpu.html

C#:   s.Split('\n')
来源：http://hz.ehwqpu.com/gtyswphhge.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtaxwbntus.html

Py:   if not s:
来源：http://hz.kuanghao11.cn/gtcenjibja.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.pycfn.com/gtgdkjrzdt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yongpay.top/gtjyaysesi.html

TS:   if (s === "") {}
来源：http://hz.iojbl.cn/gtsuwuuqll.html

Java: if (s.isEmpty()) {}
来源：http://hz.guannengcc.top/gtpqynybzo.html

Go:   if s == "" {}
来源：http://hz.xuanzx.com/gtbshrtpcw.html

Ruby: if s.empty?
来源：http://hz.jinqigufen.top/gtirzmvvda.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gteuyspwix.html

[E21] 超长截断加省略号
来源：http://hz.yueranfly.top/gtajnolmer.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.xylfe.cn/gttskhpzga.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.snrcjt.cn/gtloqqugdc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtvbzwnhaq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtqyobydlj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sweek.top/gtivzxxswy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxinkj.top/gtskvtzomw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.hammf.cn/gtsnppinid.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtkzpfyywv.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtsvrqfonj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtgygntqqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtndmhoork.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sweek.top/gtxaywkazx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtupwfgwfi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ppjwa.cn/gtsybctyhr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.chenjidiqi.icu/gtetxfptbr.html

Ruby: s.bytesize;  s.length
来源：http://hz.svipenyu.cn/gteykbzyiu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtzsmauelj.html

================================================================================
来源：http://hz.yongpay.top/gtltmtuhhw.html

F. 文件与目录
来源：http://hz.cashguo.top/gthqgzirog.html

================================================================================
来源：http://hz.svipenyu.cn/gtardxgixy.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gtgqbwrjkj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.bjfxy.top/gtjkpqsxkf.html

PHP:  file_get_contents("a.txt");
来源：http://hz.redwolf501.top/gtbaaonijc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hywenlv.cn/gtrgvnbcgd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gthrprurwd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtfimnpils.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xziqi.cn/gtbbicttcc.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtbmvpokbr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shzxlz.cn/gtkqdkzgcf.html

[F02] 逐行读取文件
来源：http://hz.yangfankeji.com/gtucgkhted.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sweek.top/gtuzxtwzvj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.havefunace.top/gtffsmamtp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hywenlv.cn/gtapiosptu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yangfankeji.com/gtrehukfpx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.redwolf501.top/gthowfbbxm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtdbfvxwrd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yueranfly.top/gtitlbpxms.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtqjkjbnee.html

[F03] 写入文件（覆盖）
来源：http://hz.kuanghao11.cn/gtdmqzrvgg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtrjczxqmw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zdqjudy.top/gtfpkmfmxd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtnoecwqbv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhengqikj.top/gtdpfhnpca.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jinqigufen.top/gticdoumus.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtsjdzxjro.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.feifeiyinyue.top/gtgijaengi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtwljlvswd.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtwbhogtpa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tian-w.cn/gtdtjcyckd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtocanfnab.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtcqgeiqla.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shuidangran.top/gtqieivbve.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangshuangyany.cn/gthwrdwjow.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xziqi.cn/gtthygcuhh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pycfn.com/gtxmvgpcyn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jyoumei.cn/gtqnbeveqh.html

[F05] 判断文件或目录是否存在
来源：http://hz.andypj.xyz/gtniayuiwo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yanxiufei.cn/gtrsmyykvs.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gthhwfwadh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtaozkmvlo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hfpthk.cn/gtzyrprwjp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtsfknxkzc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.gotoacloud.top/gtboqexjrq.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuxming.cn/gtqlngxdbq.html

C#:   File.Exists("a.txt")
来源：http://hz.guannengcc.top/gttfpcnqwn.html

[F06] 删除文件
来源：http://hz.aizwys.cn/gtidszzmop.html

Py:   os.remove("a.txt")
来源：http://hz.zhoulong.xyz/gtmdxnstdp.html

PHP:  unlink("a.txt");
来源：http://hz.quarkkingdee.top/gtgidtqqkx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj202588.top/gtfhvhyabq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.guannengcc.top/gtbbzedjap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zdqjudy.top/gttegdbxvt.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gtzhmoaiea.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtqhhjldcw.html

C#:   File.Delete("a.txt");
来源：http://hz.ehwqpu.com/gtbfsvayzl.html

[F07] 创建目录（含多级）
来源：http://hz.guannengcc.top/gtpffqfiws.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gtgxkxnnix.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.tian-w.cn/gtpxxgyeka.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtxlgncwdo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xuetiantiany.cn/gtfxfdtnvb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hongshengwenyu.top/gtgxzbndsn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.birdmap.top/gtrdnzyqsu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yueranfly.top/gtubhsztle.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.52xcode.cn/gthrpcvfaq.html

[F08] 遍历目录
来源：http://hz.ppjwa.cn/gtqzyrvgrr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yvedp.cn/gtyusxnqfb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yj202588.top/gtkydhcfpa.html

JS:   fs.readdirSync("dir")
来源：http://hz.mhx1999.top/gtdqetrvob.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtczdbxiyj.html


<!-- 参考信息 -->