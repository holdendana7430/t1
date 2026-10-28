代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.bjfxy.top/gtgrsmmdxn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtwsissgkv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtpgccycki.html

C#:   new List<int>(list);
来源：http://hz.zhixingplan.top/gtjswwfgbq.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtjsklttog.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinyuanbaomall.cn/gtzgvjeosm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtajrrqgdv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtjahwtrwf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtokgibqzn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258.top/gtcyrlbnjy.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtjteosmxp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtndccqgey.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.vqdsnc.cn/gthpadubmb.html

[D24] 字典 / Map 基本操作
来源：http://hz.daria6918.cn/gtzolcawug.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxinkj.top/gtrdzpgzoq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtzzmacass.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gtgfywfmam.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtdfyykkni.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yanxiufei.cn/gtauwizlax.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtcvogkcfb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gtcscdgryk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj20258888.top/gtwqueobbx.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gteustclfl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gtxwbmwvpr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.redwolf501.top/gtivinuviu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hongshengwenyu.top/gtgaixqyik.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtzvegzmlr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtryookbyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtzvuihmmg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtyakwrrwl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtyupzfovq.html

[D26] 数组转字符串
来源：http://hz.yj202588.top/gtfjwvqsad.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnxiangtu.top/gtwbkxpysp.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gtdohigcmi.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtuwtojwoy.html

TS:   arr.join(", ")
来源：http://hz.hysaishi.cn/gtglismstt.html

Java: String.join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtceuqngsb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhijiandao.cn/gtrklmadso.html

Ruby: arr.join(", ")
来源：http://hz.chenlongwang.top/gtzzzpunte.html

C#:   string.Join(", ", list)
来源：http://hz.jianghu66.top/gtbawwvptl.html

================================================================================
来源：http://hz.pycfn.com/gtxkltlyid.html

E. 字符串处理
来源：http://hz.zhaomingkeji.xyz/gtcksjsmfz.html

================================================================================
来源：http://hz.ehwqpu.com/gtepxnjozk.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gtgqzfihhj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhengqikj.top/gtnnzbgmlr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtxybhagdh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtetvcmjwo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gthkdqniiv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ybcxt.top/gtzggvzuvd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gogol.net.cn/gtkteivyhv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gtciwsbqqm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtfrsofnym.html

[E02] 重复字符串
来源：http://hz.gaohongyu789.top/gtlzvppdgp.html

Py:   "ab" * 3
来源：http://hz.zhongyouzk.top/gtrynatdmj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.c1oappe.top/gtabahvurp.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtjxorpfgz.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtnsaahkbm.html

Java: "ab".repeat(3)
来源：http://hz.hnqzz.top/gttjcpyyrv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangkeji.top/gtktkwuqwq.html

Ruby: "ab" * 3
来源：http://hz.jiagoushi.top/gtzgwvskjk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgufenzy.top/gtjdnmxejq.html

[E03] 截取子串
来源：http://hz.sweek.top/gtjdjcgqmr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.havefunace.top/gtixkqbkud.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhongyouzk.top/gtgphfsqop.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cqqwz.cn/gtqfqhmtnf.html

TS:   s.slice(1, 4)
来源：http://hz.tian-w.cn/gtrjnlvkdu.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtbojrmkgl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.feifeiyinyue.top/gtlsyphzdv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.52xcode.cn/gtczhkaytt.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtxtazmdez.html

[E04] 查找子串位置
来源：http://hz.wangdashe.top/gthwolpixs.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hammf.cn/gtczwyleiw.html

PHP:  strpos($s, "x");
来源：http://hz.xuetiantiany.cn/gtlbgdodmd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydzc1.top/gtvwgkwkum.html

TS:   s.indexOf("x")
来源：http://hz.dianchejie.cn/gtbemyxlgr.html

Java: s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtojudwkza.html

Go:   strings.Index(s, "x")
来源：http://hz.jlsjyb.cn/gtzqxyhoro.html

Ruby: s.index("x")
来源：http://hz.zhiwuduotai.top/gtgnkdtkhm.html

C#:   s.IndexOf("x")
来源：http://hz.nwbrower.top/gtiqnpdqrz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yangfankeji.com/gtuuagtuav.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jianghu66.top/gtpxhjlikf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yueranfly.top/gtdzfblyqr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhengqikj.top/gtxmmnrxyv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtpnxgacbr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtupzhrprt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigfzy.top/gtrgynfall.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.9152youxi.cn/gttnqfnzvi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinyuanbaomall.cn/gttoqdfvuj.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtduzohcgr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.quarkkingdee.top/gtgtvojqyr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hysaishi.cn/gtiaqzsyku.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtxuxnppsj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtebqeurmu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtqhqfyfgm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xziqi.cn/gtgdtxsxko.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cheryme.top/gtmjihjlmi.html

C#:   s.Replace("a", "b")
来源：http://hz.tian-w.cn/gtggdnaaun.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtaxkgnvsg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.vqdsnc.cn/gttpdhzfut.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnqzz.top/gtvuptesft.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtyuedhuxg.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtzkyxmnas.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ehwqpu.com/gtjtnrtnzg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hywenlv.cn/gtrarqklzt.html

Ruby: s.split(",");  s.split
来源：http://hz.jqgfzy.top/gtvvkswyle.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aibaodan.cn/gthkcmtmon.html

[E08] 数组按分隔符合并
来源：http://hz.chenzaomai.com/gtrlhkzlmk.html

Py:   ",".join(items)
来源：http://hz.shangyingyoupin.top/gtgrllopwl.html

PHP:  implode(",", $items);
来源：http://hz.hywenlv.cn/gticqyregs.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gtqnzshfof.html

TS:   items.join(",")
来源：http://hz.nwbrower.top/gtzjgmkgnz.html

Java: String.join(",", items)
来源：http://hz.jianghu66.top/gtrhdlaajo.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangkeji.top/gtrlyxujyb.html

Ruby: items.join(",")
来源：http://hz.smart0.xyz/gtnzoadkiy.html

C#:   string.Join(",", items)
来源：http://hz.sweek.top/gtfffvwlyc.html

[E09] 去除所有空白字符
来源：http://hz.shangyingyoupin.top/gtccsnnzva.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtwceubzru.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cdnleiting.top/gtivivtkpo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtmgpnhpub.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtzdawosqf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenzaomai.com/gtqcwuuuor.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pengpengdd.cyou/gtpjjosoxu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zhaomingkeji.xyz/gtcisgilpw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtltnseifo.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cdnleiting.top/gtidrfgvnc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gteoqjowqw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hongshengwenyu.top/gtdyhxvoak.html

JS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtpyazkzod.html

TS:   "7".padStart(3, "0")
来源：http://hz.gogol.net.cn/gtbfdwnuij.html

Java: String.format("%03d", 7)
来源：http://hz.cheryme.top/gtfuujgcpi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hfpthk.cn/gtcziahtra.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cqqwz.cn/gtmcibsxej.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtyxnypevf.html

[E11] 反转字符串
来源：http://hz.jinghuilouyu.cn/gtnmakywxl.html

Py:   s[::-1]
来源：http://hz.smart0.xyz/gtmkkyrvlq.html

PHP:  strrev($s);
来源：http://hz.gogol.net.cn/gtmtayivxw.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtateqaxvb.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtztgjlgok.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yueranfly.top/gtavvkgjdi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtiwwdtsme.html

Ruby: s.reverse
来源：http://hz.zhaomingkeji.xyz/gtwpjgybju.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xylfe.cn/gtxcwyhsoz.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtgzxqzuvb.html

Py:   s.count("a")
来源：http://hz.yj20258.top/gtfyhevitx.html

PHP:  substr_count($s, "a");
来源：http://hz.shangyingyoupin.top/gtflbtbxjf.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtbelwqvdt.html

TS:   s.split("a").length - 1
来源：http://hz.dashuyun.cn/gtoxuuhflm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtfvwbnjix.html

Go:   strings.Count(s, "a")
来源：http://hz.gzhubu.top/gthxhcygmc.html

Ruby: s.count("a")
来源：http://hz.chenlongwang.top/gtvbqhyinl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yj20258.top/gtmxyvppmh.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtbmkxobje.html

Py:   for ch in s: print(ch)
来源：http://hz.ppjwa.cn/gtcgvdibqt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xuanzx.com/gtcfaozgci.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtpwsdgthp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtykzfgbbo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.fzhhl.top/gtxkfptxol.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangdashe.top/gtmyaicejs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.daxiang520.top/gtkawjroly.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hysaishi.cn/gtydqhzgnc.html

[E14] URL 编码与 Base64
来源：http://hz.sufxvd.cn/gtmgklratl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fzhhl.top/gtfeutdtnk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jlsjyb.cn/gtchqzxoog.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gtacrxmoby.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtxbovlvmp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jiagoushi.top/gtslzupyco.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtzcnevnfp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cdnleiting.top/gtbyjagyld.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.c1oappe.top/gtysdpxdki.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangkeji.top/gtxdxcsuap.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhoulong.xyz/gtkjwvrcpt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinghuilouyu.cn/gtziymvgzp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.bjfxy.top/gtxpwvtudd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sysykeji.top/gtxqrlcpqv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tanke756.top/gtxxjyrwhe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtxwiboatl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtjewbhudn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhixingplan.top/gttienyymg.html

[E16] 数字千分位
来源：http://hz.jinqigufen.top/gtmvfyailz.html

Py:   f"{1234567:,}"
来源：http://hz.9152youxi.cn/gtbywvohoi.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtilekxzgv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtfgnrgnyd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtcathctuk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.svipenyu.cn/gtkrymqemm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.snrcjt.cn/gtbekyinei.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtmvwtomte.html

C#:   1234567.ToString("N0")
来源：http://hz.kuanghao11.cn/gtegdimlkb.html

[E17] 首字母大写
来源：http://hz.jinqigfzy.top/gtvgqqrblc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gaohongyu789.top/gtqvjnvkmj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtsgafbhoq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtvvrrizea.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtmnsqlpcz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtvlvujanb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangkeji.top/gtcivngyyk.html

Ruby: s.capitalize
来源：http://hz.nanxuanxn.top/gtjrcwzbon.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtgtznfayr.html

[E18] 模板占位符替换
来源：http://hz.yj20258.top/gttrrbvkyg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shzxlz.cn/gtzxdfouwb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gtzuuuqtce.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gtbrigtywm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtzvdqirqp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gtoypggkdb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhongyouzk.top/gtglppspnk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.havefunace.top/gtbvxapqou.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tianlin.xyz/gtcuwuyrlh.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtnpbdebgn.html

Py:   s.splitlines()
来源：http://hz.ydzc1.top/gtbbzmjpep.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jqgfzy.top/gtcxhpkupt.html

JS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtaqxzprik.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gtlmgajyfp.html

Java: s.lines().toList()
来源：http://hz.kuanghao11.cn/gtxwfbxuaq.html

Go:   strings.Split(s, "\n")
来源：http://hz.pycfn.com/gtkwedjhmc.html

Ruby: s.lines
来源：http://hz.yangfankeji.com/gtwbocqawa.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gthiwykeir.html

[E20] 判断字符串是否为空
来源：http://hz.hysaishi.cn/gtwphextbo.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtamilttcm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhaomingkeji.xyz/gtaiatqafr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yuanzhike.top/gtclherddn.html

TS:   if (s === "") {}
来源：http://hz.xinyue.icu/gtnntdnrtb.html

Java: if (s.isEmpty()) {}
来源：http://hz.52xcode.cn/gtqwdywbxa.html

Go:   if s == "" {}
来源：http://hz.yanxiufei.cn/gteahjerlw.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gthtedjrzy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ybcxt.top/gtpzczgqfk.html

[E21] 超长截断加省略号
来源：http://hz.hongshengwenyu.top/gtkjrtyari.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuxming.cn/gtuvvzxrtr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtwmoqmcqq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nanxuanxn.top/gtirfjczhx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnxiangtu.top/gttjpntome.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.dashuyun.cn/gtubodaikp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.shangyingyoupin.top/gtlcxgnfpu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yongpay.top/gtrzkslgtr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.daria6918.cn/gtuzkuqwho.html

[E22] 字节长度与字符长度
来源：http://hz.yueranfly.top/gtpxdmemjj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gttkgmwuva.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtyrxisvbt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.iojbl.cn/gtwimdhejd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtywputnkl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtbdxfirdp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangdashe.top/gthlkzmgpo.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuxming.cn/gtnfxidpfh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shanyushiyangkeji.top/gtqcfhbotg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtxvtorvea.html

F. 文件与目录
来源：http://hz.hfpthk.cn/gtwuukubvq.html

================================================================================
来源：http://hz.sufxvd.cn/gtbkxxtgim.html

[F01] 读取整个文件
来源：http://hz.haohaochexian.top/gtirxhfbuu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xylfe.cn/gtugcbgkxj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.vqdsnc.cn/gtxgxnplkw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinyuanbaomall.cn/gtgaribclk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gtnfwehajj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtskspnwyd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.chenzaomai.com/gteqtldgov.html

Ruby: File.read("a.txt")
来源：http://hz.yuxming.cn/gteqatchrw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.birdmap.top/gtaqgzfczn.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gtphnjrtty.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.meibo888.top/gthithqjdz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cqqwz.cn/gtwtzjyznn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtppubmhxj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtaznechqa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtbkvcrloq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtsglyvszq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.wangdashe.top/gtnyiktzid.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.havefunace.top/gtccvhpzkl.html

[F03] 写入文件（覆盖）
来源：http://hz.gzhubu.top/gtwsqpqcct.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.redwolf501.top/gtmsbnzlgs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ehwqpu.com/gtssjuenrs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shangyingyoupin.top/gtgirkqpoq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenjidiqi.icu/gtwqwqmkmn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtersvabzb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.wangdashe.top/gtrwujdiin.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xziqi.cn/gtpsbydoou.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.meibo888.top/gtrbwtntkl.html

[F04] 追加写入文件
来源：http://hz.yanxiufei.cn/gtxmwgozaw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.daria6918.cn/gtyirazlkw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dashuyun.cn/gtfizzxzzg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtsytwemmu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gtdfefuhkt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.quarkkingdee.top/gtvazhmqpx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gtwmeurbvp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yueranfly.top/gtpftfpzor.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hnqzz.top/gtjfpsqizj.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtcnbwznvf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.daxiang520.top/gtblbxnxxt.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtvenvfats.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gturdaydqo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtpmiezbsb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtqkfnvxez.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jinghuilouyu.cn/gtppjvllsr.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtwaobdfwz.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgufenzy.top/gtmqfgkyxy.html

[F06] 删除文件
来源：http://hz.jiagoushi.top/gtglgzebuw.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258888.top/gtatisxlqf.html

PHP:  unlink("a.txt");
来源：http://hz.guowangkeji.top/gtybjfciiq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtcdyvokwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgfzy.top/gtgqvhghdv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtznvimagb.html

Go:   os.Remove("a.txt")
来源：http://hz.gogol.net.cn/gtdxqbvxyf.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtgbykdgti.html

C#:   File.Delete("a.txt");
来源：http://hz.snrcjt.cn/gtlzcglsjd.html

[F07] 创建目录（含多级）
来源：http://hz.yueranfly.top/gtjexoruhv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ehwqpu.com/gtstjyhomm.html


<!-- 参考信息 -->