代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.chenzaomai.com/gtvfwpwzbu.html

JS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtcxtkysei.html

TS:   arr.includes(x)
来源：http://hz.sweek.top/gtgyfsnkfe.html

Java: list.contains(x)
来源：http://hz.hnxiangtu.top/gthddvdhef.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigfzy.top/gtcgwfcgoz.html

Ruby: arr.include?(x)
来源：http://hz.xinyue.icu/gtdleixanu.html

C#:   list.Contains(x)
来源：http://hz.chenzaomai.com/gtizhthzws.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jyoumei.cn/gtgrjpnqrj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.mhx1999.top/gtupciwfbo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangkeji.top/gtqyhpfmvb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hammf.cn/gtnfjehmaf.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtlucoamom.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtpnioeajb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gogol.net.cn/gtjtzxtypx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shuidangran.top/gtmsqchnqs.html

C#:   new List<int>(list);
来源：http://hz.tanke756.top/gtwqyiavus.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtdkpnutkw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gthgyzwatz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hongshengwenyu.top/gtsyovebgu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gthjyaxigm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gthbkauhns.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shangyingyoupin.top/gtqydbnfmo.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gttdmpmsrp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.guowangkeji.top/gtxxrhotfc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtydwgjkvm.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtylxkrwgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gteqszdkyg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtezrnuonj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gteflttylg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.birdmap.top/gtbngyolur.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yongpay.top/gtptyxmpnm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shangyingyoupin.top/gtcmuppcxn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yanxiufei.cn/gtbouittun.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fzhhl.top/gtskmwxmls.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtsgeqoprs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtjsuckszr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.aizwys.cn/gtsywaoqpt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtuvbodpus.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dianchejie.cn/gtjyndvqsd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtortuobdk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hammf.cn/gtkdzqcczl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtqlpigfib.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtikmavbnf.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtcinubcvx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtukfjksar.html

PHP:  implode(", ", $arr);
来源：http://hz.smart0.xyz/gteqvhmqki.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtyxcrdixc.html

TS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtopunwlrl.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtmweudfgu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.316326.xyz/gtalaokzws.html

Ruby: arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtsbevakxt.html

C#:   string.Join(", ", list)
来源：http://hz.hnqzz.top/gtixtdwtru.html

================================================================================
来源：http://hz.snrcjt.cn/gtbebzpatj.html

E. 字符串处理
来源：http://hz.bjfxy.top/gtczkuqiiq.html

================================================================================
来源：http://hz.sxryk.cn/gtyxirzrir.html

[E01] 拼接字符串
来源：http://hz.yonumen.top/gtmhepyccu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tian-w.cn/gtqsunvyag.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dashuyun.cn/gtoiatcgrh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtadwnixfi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtspsmqhke.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.svipenyu.cn/gtavkcuaiy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtzvdgcgje.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtmtpmpbtp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydzc1.top/gtldtolzkz.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gttijcqstm.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gtwebxtxpe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cucudq.cn/gtnanbmddd.html

JS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtwvzftwkr.html

TS:   "ab".repeat(3)
来源：http://hz.ywan-chungtsiang.top/gtknxvrqek.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtdhkcoglf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtyhoxxbkl.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtkhrvhlyl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gtfwetlrkt.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtlwoeqewa.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sufxvd.cn/gtaoybrihz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cqqwz.cn/gtpnbrmbyf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtoyfcqbjo.html

TS:   s.slice(1, 4)
来源：http://hz.yongpay.top/gtjhryzqly.html

Java: s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtykpbmsad.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jqgufenzy.top/gtouynijyg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.havefunace.top/gtqpgmpjzb.html

C#:   s.Substring(1, 3)
来源：http://hz.hysaishi.cn/gtcyhvzazh.html

[E04] 查找子串位置
来源：http://hz.yj20258888.top/gtaxjjwyys.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cdnleiting.top/gtuyknqmnj.html

PHP:  strpos($s, "x");
来源：http://hz.fengsongda.top/gtioeqobwb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.aizwys.cn/gtxldraane.html

TS:   s.indexOf("x")
来源：http://hz.bjfxy.top/gtuthlttlz.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtpilohjoh.html

Go:   strings.Index(s, "x")
来源：http://hz.jqgufenzy.top/gtsonzusmv.html

Ruby: s.index("x")
来源：http://hz.quarkkingdee.top/gtmshvsazh.html

C#:   s.IndexOf("x")
来源：http://hz.mhx1999.top/gtvwaqaiov.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yj20258888.top/gtvjbjhqdf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gtsaaswgij.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj202588.top/gtrmuqeqwj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yueranfly.top/gtilyxuppd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yueranfly.top/gtsgzwatjp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yangfankeji.com/gtylsffszc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.andypj.xyz/gtrksmzifw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhongyouzk.top/gtpygibsjf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hfpthk.cn/gtuxqnzllc.html

[E06] 替换子串
来源：http://hz.jqgfzy.top/gtxsajcxgo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cashguo.top/gtjqdixfmx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtowclfufc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtzdsvcdcl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtpenvwtea.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtiezvubpg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hnqzz.top/gtldtitiis.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.c1oappe.top/gtiaxaidez.html

C#:   s.Replace("a", "b")
来源：http://hz.sxryk.cn/gtrwaocmrc.html

[E07] 按分隔符拆分
来源：http://hz.hfpthk.cn/gtbciwtxqd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.mhx1999.top/gtvykhzaoc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangshuangyany.cn/gtpjhnlnrk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtiukbzvoy.html

TS:   s.split(",")
来源：http://hz.ehwqpu.com/gtyjejoerw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yonumen.top/gtowjmaiab.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtoglslvxe.html

Ruby: s.split(",");  s.split
来源：http://hz.fzhhl.top/gtvtiemtwh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jinghuilouyu.cn/gtpwtjrcpj.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtwyiopmtc.html

Py:   ",".join(items)
来源：http://hz.fzhhl.top/gtmrfkzdoq.html

PHP:  implode(",", $items);
来源：http://hz.guannengcc.top/gtvqjkpuht.html

JS:   items.join(",")
来源：http://hz.cashguo.top/gtqvuspodv.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gtutpzejht.html

Java: String.join(",", items)
来源：http://hz.shangyingyoupin.top/gtnfaednvz.html

Go:   strings.Join(items, ",")
来源：http://hz.guowangkeji.top/gtkaagpuzi.html

Ruby: items.join(",")
来源：http://hz.jlsjyb.cn/gtbzhawcqd.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gthctsbarp.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gtlmtnhvld.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtmynaihae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.daxiang520.top/gtclemrtfj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtzmpiqypn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtjvexqunt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yvedp.cn/gtxokjofsw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fzhhl.top/gtoioyidid.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuetiantiany.cn/gtybsibbeu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yuxming.cn/gtljumscny.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtokezabbz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xziqi.cn/gtyduvgehz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shangyingyoupin.top/gtdfydzrjd.html

JS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtoxzqxjmn.html

TS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtuhlgpfml.html

Java: String.format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtcywzeiop.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.gotoacloud.top/gtkkdmtewl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ivvv.top/gthjddwwcg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtcjckymaa.html

[E11] 反转字符串
来源：http://hz.iojbl.cn/gtntfvypxx.html

Py:   s[::-1]
来源：http://hz.zhixingplan.top/gthaquxuuo.html

PHP:  strrev($s);
来源：http://hz.hywenlv.cn/gtozoapdho.html

JS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtpwweqoka.html

TS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtsucgwldh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.cqqwz.cn/gtrujyvkqv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtpewworxe.html

Ruby: s.reverse
来源：http://hz.wangshuangyany.cn/gtfivzcjfd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.vqdsnc.cn/gthqarsceq.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gtgwxlpseo.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtesrsepyl.html

PHP:  substr_count($s, "a");
来源：http://hz.tanke756.top/gtvwtgjqde.html

JS:   s.split("a").length - 1
来源：http://hz.fzhhl.top/gtiuryfckd.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258888.top/gtdlqsskdy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gotoacloud.top/gtpqfihwbw.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gthnkmjtdk.html

Ruby: s.count("a")
来源：http://hz.jyoumei.cn/gtkxxkwrin.html

C#:   s.Count(c => c == 'a')
来源：http://hz.52xcode.cn/gtteffwyzx.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtnzjzxfbo.html

Py:   for ch in s: print(ch)
来源：http://hz.zhijiandao.cn/gthwmfjkzx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.52xcode.cn/gtizkokpww.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtapteeica.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtzhavubud.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.aibaodan.cn/gtquelauni.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtyqfifjym.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.chenjidiqi.icu/gtwajzvdxi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuxming.cn/gtywrvrcyz.html

[E14] URL 编码与 Base64
来源：http://hz.meibo888.top/gtvzweozlu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtfveppfqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtqthqifcf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yueranfly.top/gtyadcsinn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gtdlkvykjb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangshuangyany.cn/gtovvqplfa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.shanyushiyangkeji.top/gtibqazyzb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhiwuduotai.top/gtqmtmkeai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hammf.cn/gtsvabasxd.html

[E15] HTML 转义 / 反转义
来源：http://hz.ppjwa.cn/gtqoyowmfi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tianlin.xyz/gttcerxvoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.tanke756.top/gttqxtbrem.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gtcscejffx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtazghckms.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.iojbl.cn/gthisfjmyl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxuanxn.top/gtgmauvtqr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cqqwz.cn/gthatpinfg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtkldcylxy.html

[E16] 数字千分位
来源：http://hz.yvedp.cn/gtntmbpblw.html

Py:   f"{1234567:,}"
来源：http://hz.zhengqikj.top/gtjqvpxvgr.html

PHP:  number_format(1234567);
来源：http://hz.andypj.xyz/gtxdheefdu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhoulong.xyz/gtrmcwvtim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.redwolf501.top/gthdqhjvcf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gtwwbvsdjo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtmqhfuyge.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.tanke756.top/gtmivzyjdo.html

C#:   1234567.ToString("N0")
来源：http://hz.hysaishi.cn/gtfzlnjiqv.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gtawuzcprc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.svipenyu.cn/gtsikjekwc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yanxiufei.cn/gtusdubxra.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gtisnnahxh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gttgpiihui.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigufen.top/gtsrvajdsl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yj20258.top/gtmnhkszkz.html

Ruby: s.capitalize
来源：http://hz.hnqzz.top/gtrfipcorv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.kuanghao11.cn/gtggfdhhcn.html

[E18] 模板占位符替换
来源：http://hz.zhijiandao.cn/gtmjfqytat.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xylfe.cn/gtmfhtjjax.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtqtcpxbgy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtjypazjty.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtltbdrnxg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.wangshuangyany.cn/gtmzlogoop.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ppjwa.cn/gtxdwsjlgu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yj20258888.top/gtediblust.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jyoumei.cn/gtoboaykiy.html

[E19] 多行文本按行拆分
来源：http://hz.hysaishi.cn/gtuqyhtdkr.html

Py:   s.splitlines()
来源：http://hz.shanyushiyangkeji.top/gtusoronlh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtqdydacbe.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gttkjckfjo.html

TS:   s.split(/\r?\n/)
来源：http://hz.shuidangran.top/gtteklnxso.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtfkmaykbo.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtslmlwmxb.html

Ruby: s.lines
来源：http://hz.cdnleiting.top/gttklnpwsj.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtcughtgav.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtldgdrrwh.html

Py:   if not s:
来源：http://hz.guowangkeji.top/gtlvejsuvi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ivvv.top/gtigbgfnqn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gtljlninls.html

TS:   if (s === "") {}
来源：http://hz.yueranfly.top/gtmowgvbrg.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtsyuuuafi.html

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gthdaikgng.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtikbpkpnc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gtanfrwhpu.html

[E21] 超长截断加省略号
来源：http://hz.316326.xyz/gtkxautmlu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tanke756.top/gtiljtkqnu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ydzc1.top/gtnvwkzwdk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ppjwa.cn/gtkaglzprg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtephmmrto.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cucudq.cn/gtahogzzss.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtzvinkedz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenlongwang.top/gtupqmwgau.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zycfv.cn/gtbpyqeqqb.html

[E22] 字节长度与字符长度
来源：http://hz.tanke756.top/gtpteyvmie.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.snrcjt.cn/gttzgyhzvu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.haohaochexian.top/gtdhgjywch.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenzaomai.com/gtwekdjkzp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtqeatagnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnxiangtu.top/gtzooqdqtr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.cashguo.top/gtzyrwyqsh.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtprdnweig.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.cashguo.top/gtvpxkdcsg.html

================================================================================
来源：http://hz.gaohongyu789.top/gteimnprvc.html

F. 文件与目录
来源：http://hz.sxryk.cn/gthwzrseht.html

================================================================================
来源：http://hz.cdnleiting.top/gtlipfkjos.html

[F01] 读取整个文件
来源：http://hz.ydjk.org.cn/gtdrqzdard.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtjewseajv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aibaodan.cn/gtwgwiqjeh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hysaishi.cn/gtynxlhqqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtrqtykifm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtoutuemsf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cucudq.cn/gtoknwwszb.html

Ruby: File.read("a.txt")
来源：http://hz.svipenyu.cn/gtjuzxbsok.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hfpthk.cn/gtpsgbhxma.html

[F02] 逐行读取文件
来源：http://hz.jqgufenzy.top/gtmblpqioj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.bjfxy.top/gtzmkhglcq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtkacckgtq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtgiiiswzg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtsvfimkif.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtlrnwhqyc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.quarkkingdee.top/gtzzugywxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.snrcjt.cn/gtxhqvjuoe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cqqwz.cn/gtsfmmzxwg.html

[F03] 写入文件（覆盖）
来源：http://hz.chenzaomai.com/gtxwdzildf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nwbrower.top/gtstfcdghj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fzhhl.top/gtcqvvovzb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.0kj1m.cn/gtfddslwew.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtwzvvvfzc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xinyue.icu/gtaqjjqbfp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhijiandao.cn/gtevaiakba.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ppjwa.cn/gtstbcisra.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtsavjrrjm.html

[F04] 追加写入文件
来源：http://hz.0kj1m.cn/gtwjhzjkrs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.svipenyu.cn/gtumlehnuj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtocuxhdrf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.meibo888.top/gtiazaxbwk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtgdgtxiuh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.gogol.net.cn/gtdaqsmtas.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xinyue.icu/gtbgjevkxz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zycfv.cn/gtapizjlon.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinqigufen.top/gtltfxhcpy.html

[F05] 判断文件或目录是否存在
来源：http://hz.fengsongda.top/gtoowmmfkd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cheryme.top/gtfejifdlv.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtauiiwjlu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtubkvqsbt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ydjk.org.cn/gtnmvddlef.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daxiang520.top/gtlhvyrkbb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.smart0.xyz/gtqklanlzj.html

Ruby: File.exist?("a.txt")
来源：http://hz.sufxvd.cn/gtalivsmwk.html


<!-- 参考信息 -->