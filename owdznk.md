代发 wailian999

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtancdnmyq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtlrkbgnsh.html

[D21] 判断是否包含某元素
来源：http://hz.iojbl.cn/gtikslqkvu.html

Py:   x in arr
来源：http://hz.yvedp.cn/gtchjqvier.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtpohwdnqu.html

JS:   arr.includes(x)
来源：http://hz.zhixingplan.top/gtlgqfbywm.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gtzjjhxliv.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtsmrimvfs.html

Go:   slices.Contains(arr, x)
来源：http://hz.mhx1999.top/gtryyctvye.html

Ruby: arr.include?(x)
来源：http://hz.gogol.net.cn/gtfvglezcq.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtuszvnjqz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxuanxn.top/gtbyvcwhov.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hysaishi.cn/gtpzzwghsb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.smart0.xyz/gtwvazznwt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yueranfly.top/gtnviclnmh.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtzxarktmt.html

Java: new ArrayList<>(list);
来源：http://hz.hammf.cn/gtcnbqxmue.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jyoumei.cn/gtudtcawvj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jiagoushi.top/gtcpungdxg.html

C#:   new List<int>(list);
来源：http://hz.hammf.cn/gtmxvtswgh.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtjukcmurw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yongpay.top/gttdklakad.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zdqjudy.top/gtytlvxmkv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtkoykapsq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtflhxocab.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ehwqpu.com/gtdmyttlbo.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gteyavmdum.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtxpukmfcn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gzhubu.top/gttyezkdgf.html

[D24] 字典 / Map 基本操作
来源：http://hz.0kj1m.cn/gtlehixyoo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hammf.cn/gtzsyrefdt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gtdxocjpir.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhijiandao.cn/gtxfrkhmyd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.mhx1999.top/gtfavhcfhz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhixingplan.top/gtynqxcqwm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj202588.top/gtufwgyoau.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.bjfxy.top/gtceukhawf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.redwolf501.top/gtxpasmjng.html

[D25] Set 集合去重与交并差
来源：http://hz.dashuyun.cn/gtbloanmxg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtczkvkdbn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cqqwz.cn/gtgjeptnjm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinqigufen.top/gtykllsaxz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinyuanbaomall.cn/gtuhkadpde.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.dashuyun.cn/gtiiygxkcq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yongpay.top/gtighrdhmc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.smart0.xyz/gtuwsmfgxi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gtcqmzveqf.html

[D26] 数组转字符串
来源：http://hz.yangfankeji.com/gthmfalkeg.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aizwys.cn/gtjucqrtlb.html

PHP:  implode(", ", $arr);
来源：http://hz.kuanghao11.cn/gtollelscy.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gtfmocwvyx.html

TS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtuqdcrpdx.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtdkvdoont.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtrelbawpt.html

Ruby: arr.join(", ")
来源：http://hz.0kj1m.cn/gtrigcjkec.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gthqphohxg.html

================================================================================
来源：http://hz.tianlin.xyz/gtdfprhqsr.html

E. 字符串处理
来源：http://hz.xinyue.icu/gtwfiebyau.html

================================================================================
来源：http://hz.sysykeji.top/gtmlqqnbqv.html

[E01] 拼接字符串
来源：http://hz.zhoulong.xyz/gtwyqhflgq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenjidiqi.icu/gtxmcgzfcn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenlongwang.top/gtxqqlpmms.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtcyypyqux.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtwynncjjo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cucudq.cn/gtatshvsbt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtjbzyxqej.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigufen.top/gtgjiuluvn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ehwqpu.com/gtltlhfvwr.html

[E02] 重复字符串
来源：http://hz.cashguo.top/gtvvfrgbss.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gtibiheqad.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtwbbwcqch.html

JS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtdqidmhap.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtreqbapxg.html

Java: "ab".repeat(3)
来源：http://hz.xinyue.icu/gtyakrmlfw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtezeinvcu.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtzbarctft.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.andypj.xyz/gtiughlibo.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtekwrtapg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gtzihrminq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtwtfegtty.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yongpay.top/gtkjawmsiq.html

TS:   s.slice(1, 4)
来源：http://hz.hfpthk.cn/gtdmpmuxet.html

Java: s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtzknnskjf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.wangdashe.top/gtihlwttol.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ehwqpu.com/gtciuootha.html

C#:   s.Substring(1, 3)
来源：http://hz.aibaodan.cn/gtyfvnbifh.html

[E04] 查找子串位置
来源：http://hz.ivvv.top/gtqnxskqte.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtpdjmownz.html

PHP:  strpos($s, "x");
来源：http://hz.ydzc1.top/gtihbeiugv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xingfuxueyuan.xyz/gtuqblgwlj.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtaroeplja.html

Java: s.indexOf("x")
来源：http://hz.tian-w.cn/gtkpoyoake.html

Go:   strings.Index(s, "x")
来源：http://hz.shanyushiyangkeji.top/gtnqhymvai.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtpvteluuq.html

C#:   s.IndexOf("x")
来源：http://hz.daria6918.cn/gtpzaauatb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sufxvd.cn/gtulrnxhlw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtbcsmbrcc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gotoacloud.top/gtwilyoego.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.tianlin.xyz/gtodturdiq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sufxvd.cn/gtalqpawba.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gthxsankxj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.birdmap.top/gtafmrgart.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hnxiangtu.top/gtakliqeka.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtxhmlbtue.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtvdagitxb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gzhubu.top/gtbuuytngc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtunikulzb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtdqkpsbjf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.0kj1m.cn/gteesqzykb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtbzddorkg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hywenlv.cn/gtpbjmwimq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gtgfokzaoe.html

C#:   s.Replace("a", "b")
来源：http://hz.hammf.cn/gtbgxpejch.html

[E07] 按分隔符拆分
来源：http://hz.jinqigfzy.top/gttnuhpwsn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gtqxjjhwds.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yueranfly.top/gthdtwaazl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daria6918.cn/gttvbxpysa.html

TS:   s.split(",")
来源：http://hz.ydjk.org.cn/gtpxleiwiz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenlongwang.top/gtgzesfjwp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shuidangran.top/gtzodyopkt.html

Ruby: s.split(",");  s.split
来源：http://hz.feifeiyinyue.top/gthhlrgkgp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnxiangtu.top/gtktmsmwjh.html

[E08] 数组按分隔符合并
来源：http://hz.meibo888.top/gtfsbesqik.html

Py:   ",".join(items)
来源：http://hz.guannengcc.top/gtkxkgezkq.html

PHP:  implode(",", $items);
来源：http://hz.zhiwuduotai.top/gtvgxitajn.html

JS:   items.join(",")
来源：http://hz.meibo888.top/gtzptjkhbi.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gtdlwxgcob.html

Java: String.join(",", items)
来源：http://hz.ppjwa.cn/gtcxdifcue.html

Go:   strings.Join(items, ",")
来源：http://hz.jqgufenzy.top/gtsinfznkm.html

Ruby: items.join(",")
来源：http://hz.jinqigufen.top/gtwpibvhih.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtmzjgtdox.html

[E09] 去除所有空白字符
来源：http://hz.daxiang520.top/gtolqdxnbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cdnleiting.top/gtxtabvmva.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xuanzx.com/gtswcbwrhl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtriypthme.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jqgfzy.top/gtpxsecefp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenlongwang.top/gtfzwiauja.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtwanpbzvy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.vqdsnc.cn/gtmfqpqgbk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.wangdashe.top/gtgprvsqnk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gttaxxylmq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.redwolf501.top/gtrflrrite.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258.top/gtyyzfaooy.html

JS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtpqywavwj.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhijiandao.cn/gtclmwjfph.html

Java: String.format("%03d", 7)
来源：http://hz.svipenyu.cn/gtllqpamnt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ivvv.top/gtfdnlsfok.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gogol.net.cn/gtvilfwrdy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hywenlv.cn/gtmhgmaeja.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gtwklwgene.html

Py:   s[::-1]
来源：http://hz.daria6918.cn/gtqmdmgvon.html

PHP:  strrev($s);
来源：http://hz.haohaochexian.top/gtbzhtqqso.html

JS:   [...s].reverse().join("")
来源：http://hz.cashguo.top/gtnudwuqai.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtdolputiy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.guannengcc.top/gtocoucaby.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtjpxvkmmo.html

Ruby: s.reverse
来源：http://hz.ivvv.top/gtanmncylc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtionykvjt.html

[E12] 统计某字符出现次数
来源：http://hz.tian-w.cn/gtakuppeem.html

Py:   s.count("a")
来源：http://hz.nanxuanxn.top/gtqumfcvhm.html

PHP:  substr_count($s, "a");
来源：http://hz.nwbrower.top/gtqrcoumvg.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtmerxsbyx.html

TS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtslqjehqx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gogol.net.cn/gthikwxdxp.html

Go:   strings.Count(s, "a")
来源：http://hz.yonumen.top/gtbbyofjsl.html

Ruby: s.count("a")
来源：http://hz.ybcxt.top/gtgyiksoxl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinqigufen.top/gtcoqmehvo.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtqvkcdzjg.html

Py:   for ch in s: print(ch)
来源：http://hz.nwbrower.top/gtcqsurnrb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.haohaochexian.top/gtolszsknf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinghuilouyu.cn/gtloneijdi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtpgmrtean.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gtnwiunrhw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhaomingkeji.xyz/gtocuhzpan.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yuxming.cn/gtretisbfu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnqzz.top/gtcreibfhw.html

[E14] URL 编码与 Base64
来源：http://hz.hammf.cn/gtrgwcizpd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtsetcphqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtrvspprqe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zdqjudy.top/gtozpqdjpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sweek.top/gtanvuieky.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.chenzaomai.com/gtvzxrthjx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtywdxrxha.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.dianchejie.cn/gtznoiivrx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gtgmxbtdfz.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtldqpqgtf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yongpay.top/gtfnpklstd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sxryk.cn/gtupysxgqa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shuidangran.top/gtgcptwqhs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yuanzhike.top/gtcxzxtbij.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hammf.cn/gtcdijpysq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nwbrower.top/gtwusmswaj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fengsongda.top/gtuvsqutzj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.andypj.xyz/gtisyprmmo.html

[E16] 数字千分位
来源：http://hz.birdmap.top/gtuvwrxxle.html

Py:   f"{1234567:,}"
来源：http://hz.ywan-chungtsiang.top/gtuajeivlv.html

PHP:  number_format(1234567);
来源：http://hz.xziqi.cn/gtbpywgoin.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gtazdovisj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ywan-chungtsiang.top/gtkddtvrym.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tian-w.cn/gthjyoatat.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.havefunace.top/gtiqexkxiv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtkeodufrb.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gthwxxwxqk.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtsyegyofh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jiagoushi.top/gtwxsqzplp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtrjrmafxv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.aibaodan.cn/gtnntauobn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxinkj.top/gtukxcecgg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jiagoushi.top/gtipbagorf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tanke756.top/gtuxyaffbf.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtswftdevv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.316326.xyz/gtyaczmmxn.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtcykpzdfb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.shuidangran.top/gtqxnuxtqj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.316326.xyz/gtzwepobda.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.chenzaomai.com/gtvpzhecsq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zdqjudy.top/gtuhupogtl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cucudq.cn/gtqcdrdznj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxinkj.top/gtcbrplftv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinyuanbaomall.cn/gtqvozsjqe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yanxiufei.cn/gtvxepsoma.html

[E19] 多行文本按行拆分
来源：http://hz.daxiang520.top/gtiiiiktiz.html

Py:   s.splitlines()
来源：http://hz.zycfv.cn/gtwkpcoqld.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinqigufen.top/gttrbffhxu.html

JS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtjfsuqmqj.html

TS:   s.split(/\r?\n/)
来源：http://hz.yuxming.cn/gtnbutbxjd.html

Java: s.lines().toList()
来源：http://hz.cdnleiting.top/gtzloivgie.html

Go:   strings.Split(s, "\n")
来源：http://hz.c1oappe.top/gtnziknjsp.html

Ruby: s.lines
来源：http://hz.ehwqpu.com/gtfwkxrvst.html

C#:   s.Split('\n')
来源：http://hz.yangfankeji.com/gtqfmjzzcn.html

[E20] 判断字符串是否为空
来源：http://hz.hongshengwenyu.top/gttmcqttzc.html

Py:   if not s:
来源：http://hz.bjfxy.top/gtnseqhgyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shzxlz.cn/gtwaynllqm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangkeji.top/gtpnnrqupn.html

TS:   if (s === "") {}
来源：http://hz.fzhhl.top/gtaquqldsi.html

Java: if (s.isEmpty()) {}
来源：http://hz.ydjk.org.cn/gttkavxjcr.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtfuihihcy.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtfjgvptwh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhixingplan.top/gtgjraeooh.html

[E21] 超长截断加省略号
来源：http://hz.kuanghao11.cn/gtwcqadcpy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtdduqwqgk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.vqdsnc.cn/gtdcaysznu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtatfptyvh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtrjdqudtx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtgmaobdpf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnqzz.top/gtapwuqykv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigufen.top/gtvcregcsb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtqubdqmwo.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtpukqhbij.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.wangdashe.top/gtqckluxpb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jiagoushi.top/gthjroikkh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtkaaswvyb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtziivdiky.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.iojbl.cn/gtjvzboibw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.9152youxi.cn/gtxxcmqcre.html

Ruby: s.bytesize;  s.length
来源：http://hz.zhaomingkeji.xyz/gtjilcnybz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.feifeiyinyue.top/gtkwpqwcyi.html

================================================================================
来源：http://hz.aizwys.cn/gtfjsmrmuu.html

F. 文件与目录
来源：http://hz.yongpay.top/gtewimdnwq.html

================================================================================
来源：http://hz.daria6918.cn/gtsgjspmgu.html

[F01] 读取整个文件
来源：http://hz.tian-w.cn/gtsejliwol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pycfn.com/gtnetdqxpl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gtzbncnees.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yonumen.top/gttfudoaly.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.meibo888.top/gtciqklldr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gttxmyudet.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shuidangran.top/gtaxuqexqv.html

Ruby: File.read("a.txt")
来源：http://hz.jinqigufen.top/gttnrcwqus.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtzfnyoaed.html

[F02] 逐行读取文件
来源：http://hz.daria6918.cn/gtfcwgxqwk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.dianchejie.cn/gtiptnhvqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xuanzx.com/gtpefpuzoc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtoqlovaop.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtifhhibuy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtrcrbglkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtutucdsle.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xuetiantiany.cn/gtoorocpmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.meibo888.top/gtfhwvgnvk.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtgrswmvgc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.chenzaomai.com/gtadgoapyz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhiwuduotai.top/gtplcmpjdt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtnswmolqe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtbkanhxrw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.0kj1m.cn/gtllymdjxs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cucudq.cn/gtruruoqsj.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aizwys.cn/gtimqisbts.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtfbecxbjp.html

[F04] 追加写入文件
来源：http://hz.hfpthk.cn/gthfutymrr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.iojbl.cn/gtekomkrje.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.fengsongda.top/gtsnjmthkh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hongshengwenyu.top/gtknzkxxka.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtcltpryki.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sufxvd.cn/gtkelhxexz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yj20258888.top/gtkgcxqxpr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nanxinkj.top/gtrkoopapy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cheryme.top/gtvdtfnrsy.html

[F05] 判断文件或目录是否存在
来源：http://hz.sufxvd.cn/gtadvjjvus.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtytklefot.html

PHP:  file_exists("a.txt");
来源：http://hz.xuanzx.com/gtumrteicq.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtbhoktikr.html


<!-- 参考信息 -->