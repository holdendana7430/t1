代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhijiandao.cn/gtgxhyvjvo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtytryymyz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangtech.top/gtnzscjzhs.html

Go:   // 手写 map[T]int
来源：http://hz.cheryme.top/gttvqolpmk.html

Ruby: arr.tally
来源：http://hz.hammf.cn/gtuitakrkl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cdnleiting.top/gtlpkiipgh.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtapmmmqye.html

Py:   x in arr
来源：http://hz.sxryk.cn/gtniidylkw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hammf.cn/gtgvbbladw.html

JS:   arr.includes(x)
来源：http://hz.havefunace.top/gtiltmvnuo.html

TS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtgwzpmsaa.html

Java: list.contains(x)
来源：http://hz.smart0.xyz/gtjxlzkqxh.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gtdrbxlxxm.html

Ruby: arr.include?(x)
来源：http://hz.aibaodan.cn/gtbptbdikq.html

C#:   list.Contains(x)
来源：http://hz.hammf.cn/gthtssaefr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtduoprqrv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtaoiyyqpc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtulpqhxcx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhixingplan.top/gtnvgvmdef.html

TS:   [...arr];
来源：http://hz.shangyingyoupin.top/gtjimfhrdn.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtwssucrls.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tanke756.top/gtrwcqyqsy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.snrcjt.cn/gthhubtbad.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gthheiwsgd.html

[D23] reduce 累积计算
来源：http://hz.feifeiyinyue.top/gtwbzrmpyb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtjgvfxhqw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtxleviasq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtugaorrvt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtyrmnzcru.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtbnhzpmth.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtkxmcxegp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nwbrower.top/gtfssgvand.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtaqjosgav.html

[D24] 字典 / Map 基本操作
来源：http://hz.tianlin.xyz/gtbflqwzzw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtdtgtpsnd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtvxjhrryd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sysykeji.top/gtkdapxudz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenzaomai.com/gtuoinifzp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtowxcdfft.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cashguo.top/gtragidzim.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jyoumei.cn/gtpmspbodc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hfpthk.cn/gtdvowomfq.html

[D25] Set 集合去重与交并差
来源：http://hz.fzhhl.top/gtjqslckpw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigufen.top/gtlcegsbnh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtxoymjmmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.0kj1m.cn/gtivuibzzk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.haohaochexian.top/gtnmlnyzmq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zycfv.cn/gtshsfoelh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ywan-chungtsiang.top/gtzarvjntm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtgdtzvlrd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gttacloxxl.html

[D26] 数组转字符串
来源：http://hz.sufxvd.cn/gtiijzswxa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtrdxvsetn.html

PHP:  implode(", ", $arr);
来源：http://hz.dashuyun.cn/gtlwzrqglj.html

JS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtdzkiwcqf.html

TS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gtepkjighp.html

Java: String.join(", ", list)
来源：http://hz.gotoacloud.top/gttgmpgizq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gzhubu.top/gtbcrkeboc.html

Ruby: arr.join(", ")
来源：http://hz.tianlin.xyz/gtjsvnzkos.html

C#:   string.Join(", ", list)
来源：http://hz.9152youxi.cn/gtydmniawq.html

================================================================================
来源：http://hz.zycfv.cn/gtchqyegdf.html

E. 字符串处理
来源：http://hz.nwbrower.top/gthzwqznrs.html

================================================================================
来源：http://hz.jiagoushi.top/gttxtnlpbu.html

[E01] 拼接字符串
来源：http://hz.cucudq.cn/gtddmablxo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtsiohvoji.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.0kj1m.cn/gtgkylwukt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtnxnafktq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtwwnusqto.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hfpthk.cn/gtirjvlmty.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zdqjudy.top/gtsmivkpfv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhoulong.xyz/gtmvwumocw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuanzhike.top/gttgbxgudz.html

[E02] 重复字符串
来源：http://hz.haohaochexian.top/gtmkylttbh.html

Py:   "ab" * 3
来源：http://hz.quarkkingdee.top/gtakcicmpy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhixingplan.top/gtncgipgxx.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtjqjqbors.html

TS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtqavalmwl.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtfuibtmdw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fengsongda.top/gtunojmrzb.html

Ruby: "ab" * 3
来源：http://hz.yj20258888.top/gtobdmmcej.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuetiantiany.cn/gtvwtegorh.html

[E03] 截取子串
来源：http://hz.xinyue.icu/gtavnjiwbn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gtjfteqjpa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.52xcode.cn/gtdurafvjn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.birdmap.top/gtnosacqew.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtmvibtlhb.html

Java: s.substring(1, 4)
来源：http://hz.aizwys.cn/gtchaofqnq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hfpthk.cn/gtciwgrict.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.haohaochexian.top/gtzsfrsgrz.html

C#:   s.Substring(1, 3)
来源：http://hz.vqdsnc.cn/gtbaximyer.html

[E04] 查找子串位置
来源：http://hz.yueranfly.top/gtueianlag.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtseoxaiov.html

PHP:  strpos($s, "x");
来源：http://hz.ydjk.org.cn/gtmyugkhik.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.daxiang520.top/gttgqwniwu.html

TS:   s.indexOf("x")
来源：http://hz.xylfe.cn/gtshsqdnqv.html

Java: s.indexOf("x")
来源：http://hz.fengsongda.top/gtybwjqlby.html

Go:   strings.Index(s, "x")
来源：http://hz.jyoumei.cn/gtzrpvagez.html

Ruby: s.index("x")
来源：http://hz.smart0.xyz/gtanqcxsck.html

C#:   s.IndexOf("x")
来源：http://hz.guowangkeji.top/gtttwwlsjv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gzhubu.top/gtgkqhthwo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gthqvmckhk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhixingplan.top/gtkmjlrdyg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtwhjikeqk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtkkeviehz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jiagoushi.top/gtkyywmetk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.sysykeji.top/gtjgbqpdyj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yuxming.cn/gtijdbttns.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tanke756.top/gtbapqalkk.html

[E06] 替换子串
来源：http://hz.svipenyu.cn/gtzotqycsl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtyvpgeyaz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtsjoziemy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtpsickzxt.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtdhiybwjv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtfbnnrlka.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtvtgxhxpi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tanke756.top/gtvypcwhyz.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtchpthtyw.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtxtznjvqv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aizwys.cn/gtcavrivfj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.9152youxi.cn/gtngkocqqk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ehwqpu.com/gtissfrcaw.html

TS:   s.split(",")
来源：http://hz.nanxuanxn.top/gtfjcnwdai.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gtsxqfojly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtfacxyvdg.html

Ruby: s.split(",");  s.split
来源：http://hz.chenlongwang.top/gtvdrnyafm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtqhxhpckw.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtlisjmzso.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtxapqojrc.html

PHP:  implode(",", $items);
来源：http://hz.nanxinkj.top/gtpvjtznsn.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gtrsomctbx.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtvnhrjska.html

Java: String.join(",", items)
来源：http://hz.hysaishi.cn/gtbdneeodx.html

Go:   strings.Join(items, ",")
来源：http://hz.316326.xyz/gtnvzdmugw.html

Ruby: items.join(",")
来源：http://hz.nanxinkj.top/gtckhopadk.html

C#:   string.Join(",", items)
来源：http://hz.mhx1999.top/gtkrxlpjin.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gttfoszftu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sysykeji.top/gtlkpplren.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nanxinkj.top/gtahqlhfdc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtdkcuaqpv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gtsurwqgfi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hfpthk.cn/gtkebvjvrx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtxyrzwhcr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ydzc1.top/gtzzkjzias.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtquzusmty.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtuyhjoddr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sweek.top/gtpehdpsln.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hysaishi.cn/gtlvitsjri.html

JS:   "7".padStart(3, "0")
来源：http://hz.c1oappe.top/gtownaikiw.html

TS:   "7".padStart(3, "0")
来源：http://hz.kuanghao11.cn/gtjxnepwak.html

Java: String.format("%03d", 7)
来源：http://hz.jyoumei.cn/gtxsceotbi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hysaishi.cn/gtdjpnyjsc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jyoumei.cn/gtaaihewya.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtgywhngjf.html

[E11] 反转字符串
来源：http://hz.havefunace.top/gtddhylusc.html

Py:   s[::-1]
来源：http://hz.mhx1999.top/gtmpqhxjza.html

PHP:  strrev($s);
来源：http://hz.guannengcc.top/gtnersqicn.html

JS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtpmfxfxsm.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtwzbgjwvi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj202588.top/gtqtgwdtrx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtuplsgddd.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtopgrvybk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtvjzvmnof.html

[E12] 统计某字符出现次数
来源：http://hz.jianghu66.top/gtabeasbgv.html

Py:   s.count("a")
来源：http://hz.hysaishi.cn/gtpejxpkzx.html

PHP:  substr_count($s, "a");
来源：http://hz.hywenlv.cn/gtbwwpzcwc.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtnvsprnee.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtrnwuwwns.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jlsjyb.cn/gtbouwiykg.html

Go:   strings.Count(s, "a")
来源：http://hz.shuidangran.top/gtvapwtjwy.html

Ruby: s.count("a")
来源：http://hz.zhaomingkeji.xyz/gtilplgiuc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gaohongyu789.top/gtdmrkzpcy.html

[E13] 逐字符遍历
来源：http://hz.aibaodan.cn/gtabsogwiy.html

Py:   for ch in s: print(ch)
来源：http://hz.chenzaomai.com/gtlzesynty.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenzaomai.com/gtnlzjdqma.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yongpay.top/gtbjpfwgcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtbujjnwym.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.birdmap.top/gtnfgvjofd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtyjhttxye.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtkjxrlzqj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.316326.xyz/gtpxhcexcv.html

[E14] URL 编码与 Base64
来源：http://hz.hfpthk.cn/gtwwknjiug.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cheryme.top/gtlwyzxftc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zdqjudy.top/gtvhzbrsyo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xziqi.cn/gtbmlrrulu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.havefunace.top/gtyvsosoop.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gtufqlyfsi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xylfe.cn/gtbikpsogx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhaomingkeji.xyz/gtyyaybwbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtjetfcqpa.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinqigfzy.top/gtbumsioxm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.bjfxy.top/gtnjurfhzx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.52xcode.cn/gtnwswlctg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ppjwa.cn/gtygyhrlni.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.mhx1999.top/gtqybihjku.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.52xcode.cn/gtaqezosbn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtwawpbojt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cucudq.cn/gtkvwoopcu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangtech.top/gtklmrsfwu.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gthirnbzym.html

Py:   f"{1234567:,}"
来源：http://hz.hammf.cn/gtocbmiocf.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtgqxxqclc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dashuyun.cn/gtoxvfyfhx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtxpqlmhas.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xinyue.icu/gtntgsrvjs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yvedp.cn/gtphnwljcy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtfhbochwd.html

C#:   1234567.ToString("N0")
来源：http://hz.daria6918.cn/gtkmzljpez.html

[E17] 首字母大写
来源：http://hz.dashuyun.cn/gttqhswzbj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hywenlv.cn/gtycegkjwx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydzc1.top/gtezpdczmh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtpkkcaxrd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ybcxt.top/gtyzuilatr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.nwbrower.top/gtfhjlgaxq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jianghu66.top/gtuzicescz.html

Ruby: s.capitalize
来源：http://hz.feifeiyinyue.top/gtyclcbagc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.andypj.xyz/gtvvlakyga.html

[E18] 模板占位符替换
来源：http://hz.feifeiyinyue.top/gtbhqxcpco.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jinqigufen.top/gtuqweqktc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.snrcjt.cn/gtgufryltb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtwqfhhkdk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtvpblkmgo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuanzx.com/gtjalretph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.andypj.xyz/gtohwygrha.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangkeji.top/gtgtsewoti.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhijiandao.cn/gthirjkewf.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtqzyxtrfj.html

Py:   s.splitlines()
来源：http://hz.jinqigfzy.top/gtqcxjuapa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gaohongyu789.top/gtothowqqz.html

JS:   s.split(/\r?\n/)
来源：http://hz.52xcode.cn/gtpperdvxk.html

TS:   s.split(/\r?\n/)
来源：http://hz.hywenlv.cn/gtmtsmipwp.html

Java: s.lines().toList()
来源：http://hz.fengsongda.top/gtbapiabds.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtmpfcsdmq.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtlmlzgofd.html

C#:   s.Split('\n')
来源：http://hz.jinqigfzy.top/gtksydgjdq.html

[E20] 判断字符串是否为空
来源：http://hz.iojbl.cn/gtrudckkgy.html

Py:   if not s:
来源：http://hz.tian-w.cn/gthicfpuqx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj202588.top/gtkvgcqzue.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zycfv.cn/gtryhebtkb.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gthzrsssxp.html

Java: if (s.isEmpty()) {}
来源：http://hz.jiagoushi.top/gtpwmjrorn.html

Go:   if s == "" {}
来源：http://hz.kuanghao11.cn/gtnkgxqfzp.html

Ruby: if s.empty?
来源：http://hz.pengpengdd.cyou/gtltpxwabb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.pengpengdd.cyou/gtfojhjxfv.html

[E21] 超长截断加省略号
来源：http://hz.guannengcc.top/gtkfwzqycu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtsoibmvaa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sufxvd.cn/gtgfuxtwir.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtptuuucut.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cqqwz.cn/gtkdshatqn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shangyingyoupin.top/gtuildyfpi.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jqgufenzy.top/gttsoatwwh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gthzgzqjno.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dianchejie.cn/gtuigvagio.html

[E22] 字节长度与字符长度
来源：http://hz.zhijiandao.cn/gtshuidqbo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xylfe.cn/gtwpkmmqtq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hammf.cn/gtcuxtonfr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtanfhkxzf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtpjfbwwfk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yj20258.top/gtyieirwge.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.smart0.xyz/gtuyryqxbi.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtofdqvwkc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zycfv.cn/gtgqaerpia.html

================================================================================
来源：http://hz.meibo888.top/gtamsiemha.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gthnewkkbp.html

================================================================================
来源：http://hz.jlsjyb.cn/gtectfqzdw.html

[F01] 读取整个文件
来源：http://hz.shuidangran.top/gtxrioszob.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtaaonnaar.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtucsvpbye.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtkzvwpahv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuanzx.com/gterjzquyz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtlzqzyniz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtzoedhpfk.html

Ruby: File.read("a.txt")
来源：http://hz.jinghuilouyu.cn/gtmzwpzoey.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.nanxuanxn.top/gtzaqfkrtj.html

[F02] 逐行读取文件
来源：http://hz.hammf.cn/gtoqkkntfw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cucudq.cn/gtwllzremu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtejkwfyvw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gttekqbuqf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.quarkkingdee.top/gthzkxdnjj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shanyushiyangtech.top/gttfcsdjqk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gtcgydvgxd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtvejjoihg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtsegrinvc.html

[F03] 写入文件（覆盖）
来源：http://hz.shangyingyoupin.top/gtjzcsbfxs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cdnleiting.top/gtdlxyzyhq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtjasfbmht.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtqgeftvvk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtlszboyje.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xylfe.cn/gtohlfqyxo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gaohongyu789.top/gtpivqxsfa.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtpjcdddbc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtacjmzspw.html

[F04] 追加写入文件
来源：http://hz.nanxuanxn.top/gtbvklflqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.aizwys.cn/gtvvukidsr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtuprfclcp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhixingplan.top/gtuikxxreu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cqqwz.cn/gtvteawcqt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cheryme.top/gtsavsexhz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.birdmap.top/gtkbvubnim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jlsjyb.cn/gtlsgetzwu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ehwqpu.com/gtnobizhec.html


<!-- 参考信息 -->