代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtbbnnuidf.html

JS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtkadmhgts.html

TS:   arr.includes(x)
来源：http://hz.ehwqpu.com/gtxvhvgawg.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtuajaliak.html

Go:   slices.Contains(arr, x)
来源：http://hz.xinyue.icu/gtobkiqqhg.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtdimvahpf.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtihftbuaw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gtfuuubcfu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.sufxvd.cn/gtjbivdzon.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yvedp.cn/gtvhnolafg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fzhhl.top/gtwfajyygs.html

TS:   [...arr];
来源：http://hz.tian-w.cn/gtgvzrmojv.html

Java: new ArrayList<>(list);
来源：http://hz.wangdashe.top/gtsfeycwrf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sysykeji.top/gtnykofwww.html

Ruby: arr.dup;  arr.clone
来源：http://hz.vqdsnc.cn/gtegsvepmm.html

C#:   new List<int>(list);
来源：http://hz.zycfv.cn/gtvjpsqqil.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gtmjfjqboc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cucudq.cn/gtcjiwvrbx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydjk.org.cn/gtfgcldgvq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtfnfmvlxj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtyhvzbicr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.c1oappe.top/gtptxtbqek.html

Go:   // 手写循环
来源：http://hz.cashguo.top/gtnmlstiaw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtxohazfor.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nwbrower.top/gteyjqniik.html

[D24] 字典 / Map 基本操作
来源：http://hz.havefunace.top/gtttbmirhq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigufen.top/gtgsildanh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ybcxt.top/gtubtfbuuj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jianghu66.top/gtpmjnsazu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fengsongda.top/gtgtmawtxi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangdashe.top/gtjqiseply.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fzhhl.top/gtjkvyoyyc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.c1oappe.top/gtkqtfazuz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tianlin.xyz/gtgzfgxeyd.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtwkgojmza.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shzxlz.cn/gtgpzrerfw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.haohaochexian.top/gtrgiseofe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtjclavyou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cdnleiting.top/gtouvdwblh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtgawhgdsz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xingfuxueyuan.xyz/gtzewtglrg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtewiwbbdx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.snrcjt.cn/gtkeniweqc.html

[D26] 数组转字符串
来源：http://hz.iojbl.cn/gtbuuxlkic.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhongyouzk.top/gtwhirgfhd.html

PHP:  implode(", ", $arr);
来源：http://hz.sysykeji.top/gtrekvvmhg.html

JS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtduejnbuh.html

TS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtzrjlitxv.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtwqoljmdm.html

Go:   strings.Join(strs, ", ")
来源：http://hz.9152youxi.cn/gtauggpugv.html

Ruby: arr.join(", ")
来源：http://hz.chenlongwang.top/gtjddzejbv.html

C#:   string.Join(", ", list)
来源：http://hz.yj202588.top/gtzexbajxi.html

================================================================================
来源：http://hz.jlsjyb.cn/gtiyeqoqrx.html

E. 字符串处理
来源：http://hz.snrcjt.cn/gtuchicuxv.html

================================================================================
来源：http://hz.jyoumei.cn/gtagpqxqzn.html

[E01] 拼接字符串
来源：http://hz.ppjwa.cn/gtexgeqfsj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gttzdmdlox.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.snrcjt.cn/gtudrdojfh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtdhvxkbsa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtgharqowc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xylfe.cn/gtoqznsqqg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hongshengwenyu.top/gtuogcllgm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.guannengcc.top/gtvpgxsxim.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zdqjudy.top/gtuemthdcx.html

[E02] 重复字符串
来源：http://hz.jiagoushi.top/gtkbchszod.html

Py:   "ab" * 3
来源：http://hz.smart0.xyz/gthuagoxuh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinghuilouyu.cn/gtiqqrdsua.html

JS:   "ab".repeat(3)
来源：http://hz.ivvv.top/gtpqmjsfpb.html

TS:   "ab".repeat(3)
来源：http://hz.jlsjyb.cn/gtcplyjygx.html

Java: "ab".repeat(3)
来源：http://hz.shuidangran.top/gtqfsdnper.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yongpay.top/gtoycrnwdc.html

Ruby: "ab" * 3
来源：http://hz.cqqwz.cn/gthtwyzyux.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.sufxvd.cn/gtyacuxwqa.html

[E03] 截取子串
来源：http://hz.quarkkingdee.top/gtzyhpugyj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtooavyonn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fengsongda.top/gtzcjtqfhr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.snrcjt.cn/gtbjcieskr.html

TS:   s.slice(1, 4)
来源：http://hz.dianchejie.cn/gtqtfwqjrl.html

Java: s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtodapdlfq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nanxuanxn.top/gtkqwjwvwr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtgfsatgsy.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigufen.top/gtsughdrlt.html

[E04] 查找子串位置
来源：http://hz.yanxiufei.cn/gtqrymavcu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtyxjzvynb.html

PHP:  strpos($s, "x");
来源：http://hz.xuanzx.com/gtupybogin.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ywan-chungtsiang.top/gtnknlswat.html

TS:   s.indexOf("x")
来源：http://hz.yanxiufei.cn/gteiufzalv.html

Java: s.indexOf("x")
来源：http://hz.pycfn.com/gtygrnoqtr.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gtcbvrfeno.html

Ruby: s.index("x")
来源：http://hz.zhiwuduotai.top/gtaomjndzf.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtsmpcjjbt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.havefunace.top/gtqfszrpyp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.52xcode.cn/gtcaxxluvl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gttdoetfue.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtcofkhgxb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnxiangtu.top/gtzhttqyho.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hammf.cn/gtjniqlgaj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jqgfzy.top/gtxcswnhmt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtqzblsjer.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.9152youxi.cn/gthbnetjac.html

[E06] 替换子串
来源：http://hz.sxryk.cn/gtsktxvhye.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtxlrasicv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shuidangran.top/gtpybmdehy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtteuddnwp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtavdctufp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtcsmmtucx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daxiang520.top/gtbzwzjarb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtjicgmtwv.html

C#:   s.Replace("a", "b")
来源：http://hz.vqdsnc.cn/gtxilbijlg.html

[E07] 按分隔符拆分
来源：http://hz.svipenyu.cn/gtppcznsry.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fzhhl.top/gtmdgatrfq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hywenlv.cn/gtbcyalqrc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj20258888.top/gtvnfgckqf.html

TS:   s.split(",")
来源：http://hz.iojbl.cn/gtruxaezmb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhaomingkeji.xyz/gtwgmkdsbv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ydzc1.top/gtjyyjourn.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtjvunfsif.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yangfankeji.com/gtorwgbycw.html

[E08] 数组按分隔符合并
来源：http://hz.tianlin.xyz/gtdsapoiwo.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtlahkxape.html

PHP:  implode(",", $items);
来源：http://hz.yj202588.top/gtkksdavho.html

JS:   items.join(",")
来源：http://hz.ehwqpu.com/gtsiepmcbn.html

TS:   items.join(",")
来源：http://hz.sxryk.cn/gtfemjknkj.html

Java: String.join(",", items)
来源：http://hz.yj20258.top/gtnhzogkcb.html

Go:   strings.Join(items, ",")
来源：http://hz.shuidangran.top/gtglqipedg.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtiwkkbdzj.html

C#:   string.Join(",", items)
来源：http://hz.jqgfzy.top/gtvrptzjhv.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gtplldnrhg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ivvv.top/gtfkiwzezp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gtirmnzbqn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtzeuxyctg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtrolzasok.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangshuangyany.cn/gtkpmktmsm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.wangshuangyany.cn/gtvwgwjoue.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yvedp.cn/gtbwttbdkj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtqmkdfgkl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gzhubu.top/gtuutsjsjz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.pengpengdd.cyou/gthvfottuc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtjuenashz.html

JS:   "7".padStart(3, "0")
来源：http://hz.aizwys.cn/gtppftagby.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtokxxivyh.html

Java: String.format("%03d", 7)
来源：http://hz.svipenyu.cn/gtnqhlieks.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtyyqajpzc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daxiang520.top/gtchsjsmus.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.haohaochexian.top/gtnkowjryq.html

[E11] 反转字符串
来源：http://hz.dashuyun.cn/gtzxelohyw.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtnjfvpwqx.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtgrrpwaig.html

JS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtyhnwcdvv.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtjvlhmxah.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hfpthk.cn/gtdgxbnjou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sysykeji.top/gtneeoctbh.html

Ruby: s.reverse
来源：http://hz.yvedp.cn/gthmuduczk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnqzz.top/gtdeemqlvy.html

[E12] 统计某字符出现次数
来源：http://hz.gaohongyu789.top/gtmfwgolyj.html

Py:   s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtmhqzykxy.html

PHP:  substr_count($s, "a");
来源：http://hz.zhengqikj.top/gtrdxzydms.html

JS:   s.split("a").length - 1
来源：http://hz.tianlin.xyz/gtnmnefjhz.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gtahxrcgmc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydzc1.top/gtmuorbjou.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtfbqesdhg.html

Ruby: s.count("a")
来源：http://hz.sweek.top/gtjqsoiote.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtgcbgnore.html

[E13] 逐字符遍历
来源：http://hz.zdqjudy.top/gtadgacbhe.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtpinvotno.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tianlin.xyz/gtygbelwoh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtzpyopgrn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gtvzfakccz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtwyrzjufa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.chenzaomai.com/gtvepuulal.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtsjvjzats.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtxpumjuxl.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtyzomjbza.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuxming.cn/gtfzitujng.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gtgzilnzzn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xingfuxueyuan.xyz/gtkayniigt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtqlzoabsl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daxiang520.top/gtwqsjrfzm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daria6918.cn/gttbrrdtfw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gtkegvqsxu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sufxvd.cn/gtemubkceq.html

[E15] HTML 转义 / 反转义
来源：http://hz.sweek.top/gtjpnzoxxe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hysaishi.cn/gtzipovpsm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.gaohongyu789.top/gtdafpieiu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hywenlv.cn/gtwzetanhn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.quarkkingdee.top/gtamhlokyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xuanzx.com/gtrgkozcdi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daxiang520.top/gtdejzcsxc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gtlganykjs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnxiangtu.top/gtotsmqica.html

[E16] 数字千分位
来源：http://hz.jinghuilouyu.cn/gtwbwqywxh.html

Py:   f"{1234567:,}"
来源：http://hz.gzhubu.top/gtcfaoqovg.html

PHP:  number_format(1234567);
来源：http://hz.ydzc1.top/gtxitpctkt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gtbsbomlkn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgfzy.top/gtxdsgmpah.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.316326.xyz/gtflkojxwn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.quarkkingdee.top/gtyqpryauk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtghqfkfpb.html

C#:   1234567.ToString("N0")
来源：http://hz.yvedp.cn/gtdddjnqrv.html

[E17] 首字母大写
来源：http://hz.shanyushiyangkeji.top/gtpaiurewq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shuidangran.top/gtnmkrdhms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhaomingkeji.xyz/gtruqznkpa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtcmytgxwi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtbowktncw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.chenlongwang.top/gtkdgvbjwm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.pycfn.com/gtypcufqjw.html

Ruby: s.capitalize
来源：http://hz.nwbrower.top/gtdfldasge.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ywan-chungtsiang.top/gtsobcyhqq.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gtxqudctmn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.havefunace.top/gtljozavta.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhiwuduotai.top/gtrvuedfms.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gtehkzihgd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhiwuduotai.top/gtdrflihjt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yvedp.cn/gtzuxhdafw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtthwazdam.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gtcbyugdhr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhaomingkeji.xyz/gtrgkcgvho.html

[E19] 多行文本按行拆分
来源：http://hz.nanxinkj.top/gtwpvirizx.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtowsyhids.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ppjwa.cn/gtidtlcydd.html

JS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gtrhubsebq.html

TS:   s.split(/\r?\n/)
来源：http://hz.xziqi.cn/gthucfpnar.html

Java: s.lines().toList()
来源：http://hz.52xcode.cn/gtwwizlfvg.html

Go:   strings.Split(s, "\n")
来源：http://hz.0kj1m.cn/gtmvromfnz.html

Ruby: s.lines
来源：http://hz.smart0.xyz/gtgkvrfwuv.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gtjzqeaqic.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gtvlaalngs.html

Py:   if not s:
来源：http://hz.xziqi.cn/gtivmbrmbb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hfpthk.cn/gtgfnzutbt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cheryme.top/gtzqrcxmzf.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtgzbpikrk.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhoulong.xyz/gtjvwqfgpd.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gterkrskvl.html

Ruby: if s.empty?
来源：http://hz.shuidangran.top/gtbbvbobbb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuanzx.com/gtrqfltmar.html

[E21] 超长截断加省略号
来源：http://hz.cucudq.cn/gtkbfyscuw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shuidangran.top/gtsrfbcjhn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gtqjuupjjf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtaasdfgrw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtmhbdomrj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.sysykeji.top/gtenrspcir.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.ywan-chungtsiang.top/gtimwxpipa.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zycfv.cn/gtupfwhvrm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinqigufen.top/gtziwarzmt.html

[E22] 字节长度与字符长度
来源：http://hz.tianlin.xyz/gtspucijww.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtlvbchctf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj202588.top/gttbwkucyd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nwbrower.top/gtkpfwnpzl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtkctpusyj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtunajcfjf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jianghu66.top/gtoqqjjvxa.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtmhxbwlzn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gthocmfkty.html

================================================================================
来源：http://hz.cheryme.top/gtcqcfimtj.html

F. 文件与目录
来源：http://hz.yj202588.top/gtoreiosao.html

================================================================================
来源：http://hz.sufxvd.cn/gtjzahpqhh.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtluczdviu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.kuanghao11.cn/gthyvbdmze.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hfpthk.cn/gtqjpqvgtm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cucudq.cn/gtgrrcoxvd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yangfankeji.com/gtvnvoqefg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenlongwang.top/gtrenzcjti.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhengqikj.top/gtqgpjbzpc.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtwkjqkulw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shuidangran.top/gtlcocxgnz.html

[F02] 逐行读取文件
来源：http://hz.daxiang520.top/gtghofshtk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtnvrjvccd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cashguo.top/gtuuqfkwga.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtcdjzsnua.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtjdljgnkk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtxfirzlqv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinyuanbaomall.cn/gtcuhzntds.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cucudq.cn/gtafrwpwvr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ivvv.top/gturphtagn.html

[F03] 写入文件（覆盖）
来源：http://hz.zhiwuduotai.top/gthoexqdpi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ywan-chungtsiang.top/gtmrtfmqye.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhixingplan.top/gtyyqjzomx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtistxruju.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gttckhynll.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtcofjgedx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cqqwz.cn/gtfihejoek.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yueranfly.top/gtcdqwnixn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtyoennzir.html

[F04] 追加写入文件
来源：http://hz.cqqwz.cn/gttoghdfle.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnxiangtu.top/gtmshwkhiw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pengpengdd.cyou/gtxkawvria.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.52xcode.cn/gtrrhhcglz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhaomingkeji.xyz/gtgoptaxfz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuanzhike.top/gtzmsnvaam.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gogol.net.cn/gtwtvhnltu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.guowangkeji.top/gtdhwvqstk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.svipenyu.cn/gttxhqctyr.html

[F05] 判断文件或目录是否存在
来源：http://hz.chenlongwang.top/gttekxyjmq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenlongwang.top/gtuwpoixdj.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gtiprupxtz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtvjplhiyt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.aizwys.cn/gtojmxiwxo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtxmvipufz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgfzy.top/gtljiaiwrw.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtzylkdnkq.html


<!-- 参考信息 -->