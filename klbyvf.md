代发 wailian999

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gtdpuzbxhj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hongshengwenyu.top/gtdlrivuoz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangkeji.top/gtkwuqoarv.html

C#:   new List<int>(list);
来源：http://hz.jinghuilouyu.cn/gteijzfpdt.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtruizkbnk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zycfv.cn/gtklqewhyq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtvwebejnf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtmcftttbv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gthhkboysp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yanxiufei.cn/gtsicolnvt.html

Go:   // 手写循环
来源：http://hz.yvedp.cn/gtllvsiezh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtrvhnjzah.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtyhoznlol.html

[D24] 字典 / Map 基本操作
来源：http://hz.birdmap.top/gtjsbzxtyv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guannengcc.top/gtjxvfvece.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aibaodan.cn/gtmecfnqhx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnqzz.top/gtbfywmtfg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtomgaywrr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuanzx.com/gtyjlsbjcv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgfzy.top/gtytblhiia.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zdqjudy.top/gtngprtzkw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gtajyumzmd.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtmpnvmbzp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtnahchrkm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtexlqutpj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj20258.top/gtpqpugwqr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.kuanghao11.cn/gtbydbanpm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hfpthk.cn/gtadfabndl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hysaishi.cn/gtcfjcvqlg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhijiandao.cn/gtiididiop.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.havefunace.top/gtwhzlaick.html

[D26] 数组转字符串
来源：http://hz.aizwys.cn/gtwvoshaef.html

Py:   ", ".join(map(str, arr))
来源：http://hz.iojbl.cn/gtqvycfefg.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgufenzy.top/gtvgejazop.html

JS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtphpnqvyq.html

TS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtlnrehwho.html

Java: String.join(", ", list)
来源：http://hz.yj20258888.top/gtiqvujvou.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtwgyldgpb.html

Ruby: arr.join(", ")
来源：http://hz.iojbl.cn/gtgeqabcyk.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtqskgygqq.html

================================================================================
来源：http://hz.ybcxt.top/gtmvyklswc.html

E. 字符串处理
来源：http://hz.hysaishi.cn/gtbwanqoqc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtjerrpqjo.html

[E01] 拼接字符串
来源：http://hz.svipenyu.cn/gttdaiidpo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtlylqksam.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtudggqrki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtnvwvltvu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gttzzkqkua.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.smart0.xyz/gtrcfyibmz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtwlxinxjb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtyzvouhcc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtrwtuljlo.html

[E02] 重复字符串
来源：http://hz.xuanzx.com/gtlhidmjga.html

Py:   "ab" * 3
来源：http://hz.ydzc1.top/gtodbtzvap.html

PHP:  str_repeat("ab", 3);
来源：http://hz.meibo888.top/gtlmcnqufy.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtcqgxiwdb.html

TS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtznpmwtmt.html

Java: "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtehxcqvwq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhiwuduotai.top/gtogilrjgy.html

Ruby: "ab" * 3
来源：http://hz.dianchejie.cn/gtjlpbxvbi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cashguo.top/gtlrwzdgpn.html

[E03] 截取子串
来源：http://hz.redwolf501.top/gtgypkoile.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.hnqzz.top/gttjkzhddm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.iojbl.cn/gtcoxilqqm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtrtmykjgz.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gtyyhppcat.html

Java: s.substring(1, 4)
来源：http://hz.yj20258.top/gtkwaweirp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gthvwlbjoo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dianchejie.cn/gtqmwvvwju.html

C#:   s.Substring(1, 3)
来源：http://hz.yvedp.cn/gtuiuwxqtx.html

[E04] 查找子串位置
来源：http://hz.xuanzx.com/gttozciukj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtvqjjqeqp.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gtoeauyxms.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtwkhmgaxi.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtlbdhuypx.html

Java: s.indexOf("x")
来源：http://hz.tianlin.xyz/gtqlawrrrv.html

Go:   strings.Index(s, "x")
来源：http://hz.xingfuxueyuan.xyz/gtrwcniehp.html

Ruby: s.index("x")
来源：http://hz.havefunace.top/gtwzwmmftv.html

C#:   s.IndexOf("x")
来源：http://hz.haohaochexian.top/gtgmnbiyoh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhongyouzk.top/gtmxiazllt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nwbrower.top/gtwcnbfqqd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.kuanghao11.cn/gteypaewmu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangdashe.top/gtwmmdgdhe.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.c1oappe.top/gtmpivodrc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtbmhulaxv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuanzx.com/gtbozgwraj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hfpthk.cn/gtoinoflta.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tian-w.cn/gtjfbmofxo.html

[E06] 替换子串
来源：http://hz.birdmap.top/gtrhvqseth.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.dianchejie.cn/gtrvqplbuk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.quarkkingdee.top/gtzpghxxmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtbbgfnjmm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtrcskyztr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtngsxbaqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yongpay.top/gtowdjrpzo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.svipenyu.cn/gthivptget.html

C#:   s.Replace("a", "b")
来源：http://hz.yongpay.top/gtczqcwlqn.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtxuivgpqb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigufen.top/gtvwqfkqxp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sxryk.cn/gthxsuslvd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.316326.xyz/gtmzulkvfg.html

TS:   s.split(",")
来源：http://hz.chenlongwang.top/gtiprulxnv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yj20258.top/gtwunlvzst.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtrorjigpj.html

Ruby: s.split(",");  s.split
来源：http://hz.yongpay.top/gtbstuawfx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.gzhubu.top/gtcctsqhcl.html

[E08] 数组按分隔符合并
来源：http://hz.xylfe.cn/gtewxpqemp.html

Py:   ",".join(items)
来源：http://hz.snrcjt.cn/gtpnsjblxr.html

PHP:  implode(",", $items);
来源：http://hz.redwolf501.top/gtuvaoydsc.html

JS:   items.join(",")
来源：http://hz.ydzc1.top/gttndyqmug.html

TS:   items.join(",")
来源：http://hz.yuxming.cn/gturlaksne.html

Java: String.join(",", items)
来源：http://hz.nwbrower.top/gtcrirlkcj.html

Go:   strings.Join(items, ",")
来源：http://hz.yuanzhike.top/gtdhzcqrxj.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtlgkuomej.html

C#:   string.Join(",", items)
来源：http://hz.hysaishi.cn/gtiquykwnu.html

[E09] 去除所有空白字符
来源：http://hz.hfpthk.cn/gtqihwsgmf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.kuanghao11.cn/gtudnpvdng.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.fengsongda.top/gtpynabulv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtdjpoprih.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtxjidpwds.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtiiapvhvb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xingfuxueyuan.xyz/gtskyqntjg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinghuilouyu.cn/gtpviqnqvc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sweek.top/gtluvdfyyp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.aizwys.cn/gtyiqptugb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yuanzhike.top/gthvlbpnzh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtqnxgwdwi.html

JS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtawpgjgqi.html

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtyvzvotcv.html

Java: String.format("%03d", 7)
来源：http://hz.meibo888.top/gtcthkocdu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fengsongda.top/gtjwnzizzm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sweek.top/gttrnzajms.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jianghu66.top/gtpxgjguci.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gtjqemqfqq.html

Py:   s[::-1]
来源：http://hz.wangshuangyany.cn/gtwywvpkua.html

PHP:  strrev($s);
来源：http://hz.cheryme.top/gtmzzhmtkr.html

JS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtbbszgeut.html

TS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtuzzrinbq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtkrmepqkt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yvedp.cn/gtkkwdawrw.html

Ruby: s.reverse
来源：http://hz.yvedp.cn/gtikpaddzr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.feifeiyinyue.top/gtfferrals.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtnnvruhom.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtsqpudwix.html

PHP:  substr_count($s, "a");
来源：http://hz.hfpthk.cn/gtpizvqczh.html

JS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtwdqyskjc.html

TS:   s.split("a").length - 1
来源：http://hz.feifeiyinyue.top/gtggobpkga.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zdqjudy.top/gtvqnyptcz.html

Go:   strings.Count(s, "a")
来源：http://hz.nanxuanxn.top/gtfjqstscc.html

Ruby: s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtvxjutyrc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hongshengwenyu.top/gtpbgdpmlo.html

[E13] 逐字符遍历
来源：http://hz.hfpthk.cn/gtckkuknjh.html

Py:   for ch in s: print(ch)
来源：http://hz.feifeiyinyue.top/gtlruydtck.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtksttaftj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtqxgpysym.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtrqhnfmcv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hammf.cn/gtvzyazhtd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgufenzy.top/gtiiupmvjf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gtbzwgjhif.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.kuanghao11.cn/gtjbuhvjnb.html

[E14] URL 编码与 Base64
来源：http://hz.cqqwz.cn/gtpwupplkm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.svipenyu.cn/gtgivyadtd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gtomrqzdub.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xinyue.icu/gtukfxscve.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gtbdgqirwr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.smart0.xyz/gtdtoibmal.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtmfmjcdme.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtktzjbaxr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xziqi.cn/gtfmyalsiq.html

[E15] HTML 转义 / 反转义
来源：http://hz.gaohongyu789.top/gtjzsevxbb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtdviqtrzj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xinyue.icu/gtszfugytv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.iojbl.cn/gtlnaqmtha.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ehwqpu.com/gtdjzusryf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258888.top/gtzxilypyg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.haohaochexian.top/gtebiiyykm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.9152youxi.cn/gthdcpperz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gtrtqxeyre.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtxckenizh.html

Py:   f"{1234567:,}"
来源：http://hz.hysaishi.cn/gtdpautcqq.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtsgwxqdwi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhengqikj.top/gtcjycavqq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gtrisuaygo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fzhhl.top/gtcebmpkok.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.9152youxi.cn/gtxdxjmyro.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shanyushiyangkeji.top/gtredkmrgo.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigufen.top/gtxibiocih.html

[E17] 首字母大写
来源：http://hz.havefunace.top/gtrxrevpsz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tian-w.cn/gtgfwsxjgh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hywenlv.cn/gtbgkswvjc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtokfobzgn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yvedp.cn/gtlstpbqok.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhijiandao.cn/gtnvehtzhz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.gotoacloud.top/gtxkfrexuo.html

Ruby: s.capitalize
来源：http://hz.hfpthk.cn/gtgyphroop.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtivuweatf.html

[E18] 模板占位符替换
来源：http://hz.zhengqikj.top/gtdxegktcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtwoevpovs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yangfankeji.com/gtymyarddr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtgylwyolj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtyoslyvrv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtrgqibgvp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinghuilouyu.cn/gtzbbmvtdt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cheryme.top/gttqxjzthw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gtjogphtzp.html

[E19] 多行文本按行拆分
来源：http://hz.gzhubu.top/gtwcythiro.html

Py:   s.splitlines()
来源：http://hz.ivvv.top/gtjjeccveg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenjidiqi.icu/gtlznilowv.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtgmpoeiuo.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuanzhike.top/gtuczkzgom.html

Java: s.lines().toList()
来源：http://hz.guowangkeji.top/gtcarjzakq.html

Go:   strings.Split(s, "\n")
来源：http://hz.redwolf501.top/gtogxjhplv.html

Ruby: s.lines
来源：http://hz.xingfuxueyuan.xyz/gthfgrkyao.html

C#:   s.Split('\n')
来源：http://hz.yj20258.top/gtokryyqgv.html

[E20] 判断字符串是否为空
来源：http://hz.chenlongwang.top/gttfzfqvjn.html

Py:   if not s:
来源：http://hz.jinghuilouyu.cn/gtocvbmmjg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuxming.cn/gtvjfqdeaf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtrpejkjcb.html

TS:   if (s === "") {}
来源：http://hz.aibaodan.cn/gtyoqlikba.html

Java: if (s.isEmpty()) {}
来源：http://hz.smart0.xyz/gtqjjecbdn.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangtech.top/gtgekfcovg.html

Ruby: if s.empty?
来源：http://hz.havefunace.top/gtjjlpxpil.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtbpeqkzmg.html

[E21] 超长截断加省略号
来源：http://hz.xuetiantiany.cn/gtclfzsheb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.0kj1m.cn/gtcbvaqtnh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tanke756.top/gtxsaetsly.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtqoaftxgo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtkmkjulyp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.kuanghao11.cn/gtqasoikby.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.52xcode.cn/gtctaolleb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jyoumei.cn/gtevyyysik.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.xziqi.cn/gtxoagkfds.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gtacgzjbqy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.andypj.xyz/gtodoifbsr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.havefunace.top/gtzymhrkwc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guowangkeji.top/gtpyzgplca.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtpidfkrlt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtekrsrvfb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.havefunace.top/gtqyvclpzm.html

Ruby: s.bytesize;  s.length
来源：http://hz.redwolf501.top/gtolrvxend.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.kuanghao11.cn/gtguokixla.html

================================================================================
来源：http://hz.aizwys.cn/gtsigvkkgu.html

F. 文件与目录
来源：http://hz.xinyue.icu/gtnxodmvck.html

================================================================================
来源：http://hz.mhx1999.top/gtuekcodma.html

[F01] 读取整个文件
来源：http://hz.fengsongda.top/gtogegusjc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.andypj.xyz/gthcpbrgfh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtknhozvyp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj202588.top/gtovzfmukx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtdrshdazg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yuxming.cn/gtddjokclx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.dashuyun.cn/gtekdjgsuq.html

Ruby: File.read("a.txt")
来源：http://hz.guowangkeji.top/gtlmqcyswp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.guowangkeji.top/gtwmgqmoss.html

[F02] 逐行读取文件
来源：http://hz.zhongyouzk.top/gtoscuytgj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ywan-chungtsiang.top/gtuibtzgtz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.quarkkingdee.top/gtdpqhuvym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydjk.org.cn/gtlasytxsm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangdashe.top/gtwmbphkgn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.snrcjt.cn/gttwivkyib.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.fzhhl.top/gtqnpjmwpr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cdnleiting.top/gtnjxmxeiy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtfgtngzii.html

[F03] 写入文件（覆盖）
来源：http://hz.gotoacloud.top/gtclhbbope.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.fzhhl.top/gtdtghpfzv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nwbrower.top/gtomfivalz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtljsbovbt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtvhomghvb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.daria6918.cn/gtiajjgqmu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hywenlv.cn/gtcfukuzmw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gzhubu.top/gtjoqnilrr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.smart0.xyz/gtkiodtnun.html

[F04] 追加写入文件
来源：http://hz.zhijiandao.cn/gtpomavmqv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cqqwz.cn/gtfajhfymm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pycfn.com/gtvtjivcmw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtlofheqbt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtwacrbhzp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtdshsrgmc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cheryme.top/gtlhbfcntc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258888.top/gtfubyjvbx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ywan-chungtsiang.top/gticapfopa.html

[F05] 判断文件或目录是否存在
来源：http://hz.meibo888.top/gtkidarnmj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xuanzx.com/gtzzxdifzj.html

PHP:  file_exists("a.txt");
来源：http://hz.yvedp.cn/gtxvuxernc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtuydqbpvq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gttaymjyes.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtjihacfwb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.hnxiangtu.top/gtghjfcegr.html

Ruby: File.exist?("a.txt")
来源：http://hz.quarkkingdee.top/gtudbkdpsx.html

C#:   File.Exists("a.txt")
来源：http://hz.yvedp.cn/gtdajszuxc.html

[F06] 删除文件
来源：http://hz.birdmap.top/gtuxesrqbp.html

Py:   os.remove("a.txt")
来源：http://hz.andypj.xyz/gtttlztnuz.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtlkrwdgtm.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.9152youxi.cn/gtpdfjvrjr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtbbwibzgc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtjypiztrm.html

Go:   os.Remove("a.txt")
来源：http://hz.gaohongyu789.top/gteafopxeo.html

Ruby: File.delete("a.txt")
来源：http://hz.shzxlz.cn/gtdwdbdorc.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtyxkrvvbl.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258.top/gtqkucrfic.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cdnleiting.top/gtzjnadalo.html


<!-- 参考信息 -->