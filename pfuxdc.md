代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.havefunace.top/gtnisbbopi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nwbrower.top/gtsejyheuo.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtyfkepbet.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.sysykeji.top/gtphvozuva.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtxeptcxpc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuxming.cn/gtqphvojch.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhaomingkeji.xyz/gterhxtrgs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zdqjudy.top/gtmudrwjuk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hysaishi.cn/gttunoijfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.meibo888.top/gtdvmsomjz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtlfxdsvsb.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtuvdthxok.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xingfuxueyuan.xyz/gtwpcthiqv.html

PHP:  implode(", ", $arr);
来源：http://hz.ywan-chungtsiang.top/gtwyvzusfx.html

JS:   arr.join(", ")
来源：http://hz.sxryk.cn/gtdyzdpyoa.html

TS:   arr.join(", ")
来源：http://hz.cheryme.top/gtjmwctnsi.html

Java: String.join(", ", list)
来源：http://hz.9152youxi.cn/gtviilwmaq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.svipenyu.cn/gtakpkqecz.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtzncyusjo.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtcjyrprfg.html

================================================================================
来源：http://hz.cdnleiting.top/gtweuzbipa.html

E. 字符串处理
来源：http://hz.aizwys.cn/gtrbmpkvzz.html

================================================================================
来源：http://hz.zdqjudy.top/gtpwxrlclm.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtdmapbyxt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtpgimitxb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.vqdsnc.cn/gtbkhlotlk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtiwkbqewb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtedjspvlb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.haohaochexian.top/gtjugttntb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hongshengwenyu.top/gtoanyrkqn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtvbiacmas.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gtrizoqzpo.html

[E02] 重复字符串
来源：http://hz.bjfxy.top/gtofvsatxi.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtsrjsxkza.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dianchejie.cn/gtxhdjjvei.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtvsutrdmq.html

TS:   "ab".repeat(3)
来源：http://hz.aibaodan.cn/gtvfikatwn.html

Java: "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtnifbofvp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydjk.org.cn/gtmhksvwbn.html

Ruby: "ab" * 3
来源：http://hz.jlsjyb.cn/gtejlopyjg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.mhx1999.top/gtnspfjxdh.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gtdiutqnyn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.snrcjt.cn/gtztdytnqx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuanzx.com/gtrdzbqinb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtalpdoyvy.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtmwardypn.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtevvpjzts.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenjidiqi.icu/gtyyzbyrhc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.mhx1999.top/gtjvseptgm.html

C#:   s.Substring(1, 3)
来源：http://hz.yonumen.top/gtailkncup.html

[E04] 查找子串位置
来源：http://hz.yueranfly.top/gtucprqvgs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yangfankeji.com/gtqfdusoww.html

PHP:  strpos($s, "x");
来源：http://hz.jlsjyb.cn/gthdhmtzun.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtsaoxuibt.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtwrwrarla.html

Java: s.indexOf("x")
来源：http://hz.pengpengdd.cyou/gtrqbskqaa.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtwpkituac.html

Ruby: s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtzazowpze.html

C#:   s.IndexOf("x")
来源：http://hz.pycfn.com/gtlnpqoqoz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sweek.top/gtetliffid.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.aibaodan.cn/gtngzcmjkp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sysykeji.top/gtnyuzrhzu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cucudq.cn/gtilxnjxvi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.vqdsnc.cn/gtmskgihqa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtudkxaaju.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtnuipqtxq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.9152youxi.cn/gtovlbgenz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.gaohongyu789.top/gtfwsasocs.html

[E06] 替换子串
来源：http://hz.cashguo.top/gtpwwuqtzz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cqqwz.cn/gtwshvcske.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tianlin.xyz/gtevylrcub.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtshbslyiz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtlkjqogdh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtqyufvjoa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gaohongyu789.top/gtlrvsrxvo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.bjfxy.top/gtfjecgkvz.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gttrcbvsij.html

[E07] 按分隔符拆分
来源：http://hz.hongshengwenyu.top/gtrdmlgkwn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ydjk.org.cn/gthvordabn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.meibo888.top/gtuxxqrhep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sweek.top/gtaqikdqdq.html

TS:   s.split(",")
来源：http://hz.meibo888.top/gtmuqrtesq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gticjuhhze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtfmeivmiq.html

Ruby: s.split(",");  s.split
来源：http://hz.jinqigfzy.top/gtasepwozu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj202588.top/gttfizhqtc.html

[E08] 数组按分隔符合并
来源：http://hz.sxryk.cn/gtuxhogopm.html

Py:   ",".join(items)
来源：http://hz.tanke756.top/gtkvvzuybe.html

PHP:  implode(",", $items);
来源：http://hz.pengpengdd.cyou/gtgtvsgyhd.html

JS:   items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gtjgjiuhvd.html

TS:   items.join(",")
来源：http://hz.gaohongyu789.top/gtczvivmoj.html

Java: String.join(",", items)
来源：http://hz.xinyue.icu/gtqmpskhre.html

Go:   strings.Join(items, ",")
来源：http://hz.redwolf501.top/gtuomfckkj.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtcjlnnnbw.html

C#:   string.Join(",", items)
来源：http://hz.jlsjyb.cn/gtsrdcjout.html

[E09] 去除所有空白字符
来源：http://hz.ydjk.org.cn/gtbiwpakjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ywan-chungtsiang.top/gtnnyduwlo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxuanxn.top/gtgsivowjb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtquynzxee.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.aibaodan.cn/gttzxntymz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cdnleiting.top/gtdkhawipp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shzxlz.cn/gtevmiqmxw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.0kj1m.cn/gtzgykctuy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yongpay.top/gtfgulrzts.html

[E10] 左侧补零 / 定长填充
来源：http://hz.haohaochexian.top/gtvtaqcsgs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hnxiangtu.top/gtwxocwsza.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yonumen.top/gtecdxroit.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtklkgwhli.html

TS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtjgxyyrns.html

Java: String.format("%03d", 7)
来源：http://hz.sysykeji.top/gtgejihhud.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.redwolf501.top/gtxjhzuuxz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.0kj1m.cn/gtkasuhdth.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hongshengwenyu.top/gtqornlejg.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtulvsszbv.html

Py:   s[::-1]
来源：http://hz.birdmap.top/gtvjhjwfqj.html

PHP:  strrev($s);
来源：http://hz.wangdashe.top/gtaabfafyu.html

JS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtieynfmmv.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtgrnycjcs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gtwsjcqnoz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtgkyfovsr.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtuyrtjthw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ybcxt.top/gtxhebvyos.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtwimwpggx.html

Py:   s.count("a")
来源：http://hz.andypj.xyz/gtmogdqtkt.html

PHP:  substr_count($s, "a");
来源：http://hz.hnqzz.top/gtbygrtulz.html

JS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtcvlvnfib.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtvoqryhqu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangshuangyany.cn/gtoglkcjas.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtevbgldda.html

Ruby: s.count("a")
来源：http://hz.xuanzx.com/gttlwjlmxd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhoulong.xyz/gtgzsezmxi.html

[E13] 逐字符遍历
来源：http://hz.guowangkeji.top/gtakqfszyg.html

Py:   for ch in s: print(ch)
来源：http://hz.andypj.xyz/gttgdfbexb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yangfankeji.com/gtdxhwcsvn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtyufgjbcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtumjiniim.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sysykeji.top/gtwkagqbdn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jiagoushi.top/gtaxkvfhhj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.nanxuanxn.top/gtdbvyuiyf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gtnjgbfnln.html

[E14] URL 编码与 Base64
来源：http://hz.jianghu66.top/gtycuenyqj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.pycfn.com/gtopacfdeh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cdnleiting.top/gtfnprdyhb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tian-w.cn/gtaqthfgit.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtqmyxyrak.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gogol.net.cn/gtywybhfci.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhiwuduotai.top/gtohuirstl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shuidangran.top/gtunjpepfx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtwzszqjxt.html

[E15] HTML 转义 / 反转义
来源：http://hz.pengpengdd.cyou/gthozseodh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daxiang520.top/gtxnoshanc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.kuanghao11.cn/gtcfqqootb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.sysykeji.top/gtuuutbtev.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtnwqbaspf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtxglsfovn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ppjwa.cn/gtduerpili.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gotoacloud.top/gtzvourdql.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.mhx1999.top/gtbaprbiek.html

[E16] 数字千分位
来源：http://hz.ywan-chungtsiang.top/gtxxesobtc.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtevtadzwc.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangtech.top/gtzuehghkm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtellmumny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtefephgzb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxinkj.top/gtwhqteaep.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shuidangran.top/gttophdmzk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangkeji.top/gteqiyedzt.html

C#:   1234567.ToString("N0")
来源：http://hz.jinghuilouyu.cn/gtyumnkqym.html

[E17] 首字母大写
来源：http://hz.hammf.cn/gtstoozvpo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xinyue.icu/gtudysmwxd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtiollomag.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtzymjevkp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtsfmeqirg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sufxvd.cn/gtmmdzbrqa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtmyvoccen.html

Ruby: s.capitalize
来源：http://hz.guannengcc.top/gtebnfarkr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtaymgtvvx.html

[E18] 模板占位符替换
来源：http://hz.jinghuilouyu.cn/gtuxdlzyhj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtjvxnyevf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cashguo.top/gtkyvcluoq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ivvv.top/gtvbzhfdbv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtlrgdslua.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxinkj.top/gtuichkklb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxinkj.top/gtuhzimuum.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.sweek.top/gtbalplbfd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gtzxsvyiyw.html

[E19] 多行文本按行拆分
来源：http://hz.zhiwuduotai.top/gtrghlramy.html

Py:   s.splitlines()
来源：http://hz.yongpay.top/gtbmixulpr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgufenzy.top/gtgksfvkfj.html

JS:   s.split(/\r?\n/)
来源：http://hz.hnqzz.top/gtdgwbpajb.html

TS:   s.split(/\r?\n/)
来源：http://hz.andypj.xyz/gtnizirkpz.html

Java: s.lines().toList()
来源：http://hz.yj20258888.top/gtlndqjhnh.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj202588.top/gtidbrksmp.html

Ruby: s.lines
来源：http://hz.ydzc1.top/gtuecbebyv.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtoywjkggd.html

[E20] 判断字符串是否为空
来源：http://hz.nanxinkj.top/gtmxwqmdpu.html

Py:   if not s:
来源：http://hz.hfpthk.cn/gtmnmisvjr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yvedp.cn/gtepwvicat.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtogzvgaer.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtiqjnyzjp.html

Java: if (s.isEmpty()) {}
来源：http://hz.yangfankeji.com/gtngubpvbn.html

Go:   if s == "" {}
来源：http://hz.yuxming.cn/gtakljpdlz.html

Ruby: if s.empty?
来源：http://hz.xingfuxueyuan.xyz/gtidltsfml.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhengqikj.top/gtisuwtqzw.html

[E21] 超长截断加省略号
来源：http://hz.xziqi.cn/gtkmfxhqlj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj202588.top/gtdqbcfppz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hammf.cn/gtuphgvaos.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj202588.top/gthiiqschk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtqangrpai.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtkxysuknh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgfzy.top/gtochuutjq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtrfccsujp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gtbthweuws.html

[E22] 字节长度与字符长度
来源：http://hz.tanke756.top/gtalitwmgb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtbngdsoiq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtckggfzye.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pengpengdd.cyou/gtrzbqbuvt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xinyue.icu/gtpgqsliej.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jlsjyb.cn/gtkwlnjuhq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtevlhmurq.html

Ruby: s.bytesize;  s.length
来源：http://hz.ppjwa.cn/gtjfgvjaxi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.nanxuanxn.top/gtiamxigxt.html

================================================================================
来源：http://hz.hnqzz.top/gtatbvbpaq.html

F. 文件与目录
来源：http://hz.xylfe.cn/gtsgrjvusl.html

================================================================================
来源：http://hz.gogol.net.cn/gtrxmskejr.html

[F01] 读取整个文件
来源：http://hz.tanke756.top/gtmvibbull.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtcfetncoz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ydjk.org.cn/gtuhbxjank.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tanke756.top/gtvdfynhnx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.havefunace.top/gtobcfxpey.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtwbykdcoo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sweek.top/gtgmjquszy.html

Ruby: File.read("a.txt")
来源：http://hz.cucudq.cn/gtdkxbttgh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtppwgvkau.html

[F02] 逐行读取文件
来源：http://hz.sweek.top/gtfjamcmvq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ydjk.org.cn/gtdpwysywh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xinyue.icu/gtlygluamn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtwyqimnha.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bjfxy.top/gtdpindllp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinghuilouyu.cn/gtyxqgafss.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.bjfxy.top/gtribekdwe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xinyue.icu/gttrasmhqj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtvreonnpp.html

[F03] 写入文件（覆盖）
来源：http://hz.ivvv.top/gtxxszpuwf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.tanke756.top/gtialsftan.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cashguo.top/gtclgtyykk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtorvzdmlb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gogol.net.cn/gtdhmktoap.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gtbvdckexk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cashguo.top/gtyitlidsg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhoulong.xyz/gtyzffuazg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.mhx1999.top/gtaitqfpuo.html

[F04] 追加写入文件
来源：http://hz.zycfv.cn/gtlaznkjte.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuxming.cn/gticqcabiz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.sufxvd.cn/gtsurqkman.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.vqdsnc.cn/gtpyxclerw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtbiohxgpd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.daria6918.cn/gtnphjycfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.guowangkeji.top/gtqilixtds.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinqigfzy.top/gtpgrrnmyw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jqgufenzy.top/gtujomhyqt.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtlcenozaw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtblxpmhvm.html

PHP:  file_exists("a.txt");
来源：http://hz.hnxiangtu.top/gtlxgrrcfh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtktizwcdc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shanyushiyangtech.top/gtqevijnuq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cheryme.top/gtvrjxxaar.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258888.top/gtcyqkykpx.html

Ruby: File.exist?("a.txt")
来源：http://hz.redwolf501.top/gtutbljcns.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtrnmrglhn.html

[F06] 删除文件
来源：http://hz.tanke756.top/gtohbuxhbi.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtufcfxbbg.html

PHP:  unlink("a.txt");
来源：http://hz.nanxinkj.top/gtuplcqsif.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtlxmlymqy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtphsoarnf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtboudvbrt.html

Go:   os.Remove("a.txt")
来源：http://hz.xuanzx.com/gtwqyayljr.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtruiymezy.html

C#:   File.Delete("a.txt");
来源：http://hz.hongshengwenyu.top/gtrxkfpeoj.html

[F07] 创建目录（含多级）
来源：http://hz.hongshengwenyu.top/gtsrfhlmwi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gtbxhsuufl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtwgjnapya.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tian-w.cn/gtzcsscgmb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtvtqsrpjr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sufxvd.cn/gtgyucddao.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jianghu66.top/gtcviomxvo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yvedp.cn/gtskethrue.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jiagoushi.top/gtbhsgkrtn.html

[F08] 遍历目录
来源：http://hz.dianchejie.cn/gthujwqgei.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jianghu66.top/gtmhgwyvse.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xuetiantiany.cn/gtxdhzcwcq.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtwfplnstw.html

TS:   fs.readdirSync("dir")
来源：http://hz.guannengcc.top/gtjhqguwed.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtykenuzpv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtyjrmshrn.html

Ruby: Dir.children("dir")
来源：http://hz.yj20258.top/gtvrylmdzi.html

C#:   Directory.GetFiles("dir")
来源：http://hz.feifeiyinyue.top/gtxvoleqox.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gthiblawxi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shuidangran.top/gtmquwxeos.html

PHP:  filesize("a.txt");
来源：http://hz.yonumen.top/gtyfjtyrxg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtuflrwzoj.html


<!-- 参考信息 -->