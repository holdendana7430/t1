代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtoazzekic.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtsvoquzcr.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtqhptzutq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yangfankeji.com/gttgdqmbnq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.feifeiyinyue.top/gtmblqgubu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtudujidku.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenzaomai.com/gtumggidpm.html

TS:   [...arr];
来源：http://hz.jinqigufen.top/gtabrhdkqk.html

Java: new ArrayList<>(list);
来源：http://hz.zhengqikj.top/gthfuyhqah.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.kuanghao11.cn/gtdaljflkp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ivvv.top/gtoejlkjze.html

C#:   new List<int>(list);
来源：http://hz.jinqigfzy.top/gtqrhjqfqp.html

[D23] reduce 累积计算
来源：http://hz.snrcjt.cn/gtxowhiajx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ppjwa.cn/gttjbmexyz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yongpay.top/gtbwnaktnf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtsfkezxik.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtanqpfkqr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hysaishi.cn/gtxhqgdgko.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtazglcbym.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangkeji.top/gtkzwnloxr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtscbjfpug.html

[D24] 字典 / Map 基本操作
来源：http://hz.wangdashe.top/gtvenenwvy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zycfv.cn/gtmyswmqqj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtzujukuth.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xylfe.cn/gtvcckkrld.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gttrviijfq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dashuyun.cn/gtmlkjpxfu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gthnfpyocm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xuetiantiany.cn/gtnttfocyq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuanzhike.top/gtlgzxlztx.html

[D25] Set 集合去重与交并差
来源：http://hz.iojbl.cn/gtnttuvnuz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.pycfn.com/gtcqpzvhko.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtnwhjfzgz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydjk.org.cn/gtbmpnkfeu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ybcxt.top/gttrrkpori.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydzc1.top/gtvhwlpape.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jlsjyb.cn/gtabprtfvt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gzhubu.top/gtroonkbzb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjfxy.top/gtchooxbid.html

[D26] 数组转字符串
来源：http://hz.sufxvd.cn/gthisuocsi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtjmteljfe.html

PHP:  implode(", ", $arr);
来源：http://hz.c1oappe.top/gttagchhtb.html

JS:   arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtwcigjxoj.html

TS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtjsagvfta.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtxfjdujwh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtcdxbkabv.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gtmlxckxlp.html

C#:   string.Join(", ", list)
来源：http://hz.quarkkingdee.top/gtbikqqilb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkdjmhvpi.html

E. 字符串处理
来源：http://hz.jinyuanbaomall.cn/gtsczjorjy.html

================================================================================
来源：http://hz.aibaodan.cn/gtqbbrvcmt.html

[E01] 拼接字符串
来源：http://hz.c1oappe.top/gtbmkzovpc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sufxvd.cn/gtonkbqcyi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigfzy.top/gtijrhtegk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtfthxgptc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtgvfbjblb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtrhqcwrak.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangkeji.top/gtilldrrhp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gtnrkivuab.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gtwyxybztf.html

[E02] 重复字符串
来源：http://hz.jiagoushi.top/gtgcgtimzs.html

Py:   "ab" * 3
来源：http://hz.jinqigfzy.top/gtixoibhex.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gtxxcgqizg.html

JS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gtzkdpqkgm.html

TS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtmepnstnj.html

Java: "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtudizvaji.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hongshengwenyu.top/gtevxjktsv.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtlfkgetst.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gtyvijncky.html

[E03] 截取子串
来源：http://hz.ivvv.top/gtkyzglmfy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.havefunace.top/gtizgpcewj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhiwuduotai.top/gthwypjgrs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.316326.xyz/gtnpimlthx.html

TS:   s.slice(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtgtqgwuyo.html

Java: s.substring(1, 4)
来源：http://hz.mhx1999.top/gtchfauoeu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhaomingkeji.xyz/gtlixurrfw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangdashe.top/gtsaatlapk.html

C#:   s.Substring(1, 3)
来源：http://hz.hnqzz.top/gtyjkiyfdx.html

[E04] 查找子串位置
来源：http://hz.zdqjudy.top/gtxahvlqzd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sufxvd.cn/gtuluoanmk.html

PHP:  strpos($s, "x");
来源：http://hz.xinyue.icu/gtmnphrjma.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenlongwang.top/gtyuyznlne.html

TS:   s.indexOf("x")
来源：http://hz.c1oappe.top/gtxrbyzjvt.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gtccbnftyb.html

Go:   strings.Index(s, "x")
来源：http://hz.sweek.top/gtxldkchyw.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gtmraquejs.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtanhzjvfe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxinkj.top/gtxifahzgq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gtsjgsjjun.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ywan-chungtsiang.top/gttvwyimtx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.feifeiyinyue.top/gtscvchndr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtlnpjilau.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sufxvd.cn/gtakojjlym.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydzc1.top/gtpnsjbwxt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yonumen.top/gtekdannzf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gtixthxctp.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtuanqjchw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shzxlz.cn/gtfpibmadl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.kuanghao11.cn/gtetggbdpq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtzrlgkgzg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtomjphcrj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtglopdjpj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj202588.top/gtmzitwxps.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yangfankeji.com/gtsrnqqhtb.html

C#:   s.Replace("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtlxgiobdp.html

[E07] 按分隔符拆分
来源：http://hz.daria6918.cn/gtjjhtuhdy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jiagoushi.top/gtdabvfwsm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xziqi.cn/gtfcpedcap.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhaomingkeji.xyz/gtqpmucvcw.html

TS:   s.split(",")
来源：http://hz.yonumen.top/gtaidwgsty.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cucudq.cn/gtvflixqdx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtrwaypjxr.html

Ruby: s.split(",");  s.split
来源：http://hz.tanke756.top/gtrhrnwyjj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hfpthk.cn/gtzppfnhjs.html

[E08] 数组按分隔符合并
来源：http://hz.snrcjt.cn/gtpkpmypdg.html

Py:   ",".join(items)
来源：http://hz.pengpengdd.cyou/gtgeevtlab.html

PHP:  implode(",", $items);
来源：http://hz.zhoulong.xyz/gtreaweawq.html

JS:   items.join(",")
来源：http://hz.redwolf501.top/gtocrganym.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gtzoeykowl.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtinhasrpn.html

Go:   strings.Join(items, ",")
来源：http://hz.xziqi.cn/gtbshdincb.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangtech.top/gtnojiwnqy.html

C#:   string.Join(",", items)
来源：http://hz.zhijiandao.cn/gtlxxsrtoy.html

[E09] 去除所有空白字符
来源：http://hz.hnqzz.top/gtkvonisxr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gaohongyu789.top/gtigahgkuf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.0kj1m.cn/gtplifhodh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtnohcavez.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtowiikyrp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jqgfzy.top/gtluimeoyw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sysykeji.top/gtwidskutx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hongshengwenyu.top/gtmrtmpzrl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zycfv.cn/gtzmqkmudu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gthhaxxazs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj20258.top/gtkknavrgq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hongshengwenyu.top/gtotyudmyy.html

JS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtlmchvhps.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtlbswedis.html

Java: String.format("%03d", 7)
来源：http://hz.ehwqpu.com/gthuvjvtua.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ppjwa.cn/gtnffgolrj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gtgdafxrup.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jiagoushi.top/gtpvalsxmc.html

[E11] 反转字符串
来源：http://hz.sxryk.cn/gtewnexjyc.html

Py:   s[::-1]
来源：http://hz.ydjk.org.cn/gtwxhqoclf.html

PHP:  strrev($s);
来源：http://hz.jiagoushi.top/gtorxoxevx.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigufen.top/gttffjlync.html

TS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtzhzwumdq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtmzlesnus.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtazkiawsv.html

Ruby: s.reverse
来源：http://hz.feifeiyinyue.top/gtxdynpzgr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.birdmap.top/gtanlujzqo.html

[E12] 统计某字符出现次数
来源：http://hz.52xcode.cn/gtzuojjdmg.html

Py:   s.count("a")
来源：http://hz.hammf.cn/gtugsypxym.html

PHP:  substr_count($s, "a");
来源：http://hz.yangfankeji.com/gtfvqeunqw.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtscxwjvtw.html

TS:   s.split("a").length - 1
来源：http://hz.svipenyu.cn/gtdatdzdpt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.quarkkingdee.top/gtzvxjobnj.html

Go:   strings.Count(s, "a")
来源：http://hz.yonumen.top/gtjxzvjcmf.html

Ruby: s.count("a")
来源：http://hz.fengsongda.top/gtehhemkhw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yanxiufei.cn/gtxmnixbgc.html

[E13] 逐字符遍历
来源：http://hz.yanxiufei.cn/gtiupsvoxf.html

Py:   for ch in s: print(ch)
来源：http://hz.havefunace.top/gtlcgtofch.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinyuanbaomall.cn/gthtgijele.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtlokllpyh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtwqofhbrp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtfonhhnaa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangshuangyany.cn/gtyhltqurn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhaomingkeji.xyz/gtkwjfbchh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aibaodan.cn/gtqbshqocl.html

[E14] URL 编码与 Base64
来源：http://hz.shangyingyoupin.top/gtfvwywujs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtvljpltqp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gtckojbewb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xinyue.icu/gtebwtmlud.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtnuyiyjgu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtklxmwshd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtuqkcoyto.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtyrlluqdx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhengqikj.top/gtshgedens.html

[E15] HTML 转义 / 反转义
来源：http://hz.pycfn.com/gtvwvbjgzc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hnxiangtu.top/gtswiqejri.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zycfv.cn/gtzkrwghkr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtxegxrzbw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.316326.xyz/gtmincrlvi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hnxiangtu.top/gtnhgvqvto.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtshyhldtg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tianlin.xyz/gteinpvccj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtfnpamrht.html

[E16] 数字千分位
来源：http://hz.snrcjt.cn/gtxzugyzwf.html

Py:   f"{1234567:,}"
来源：http://hz.52xcode.cn/gtsbcpolib.html

PHP:  number_format(1234567);
来源：http://hz.ppjwa.cn/gtklhxqbpa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtmtksvdbr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jianghu66.top/gtxpjhxuay.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.feifeiyinyue.top/gtaollrzkl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ivvv.top/gtsnwuydfc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dashuyun.cn/gtsjcznvzh.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtjumujzqq.html

[E17] 首字母大写
来源：http://hz.xuetiantiany.cn/gtzmyjnfab.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hfpthk.cn/gtcybqtwzf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.wangshuangyany.cn/gtzlyndvvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gtfworxbpc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.haohaochexian.top/gtrjiaytyv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtvdysnigc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenzaomai.com/gteqcebacf.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gtsifbuxoi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ydzc1.top/gtppavlvke.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtpjffgjhq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.svipenyu.cn/gtnsnofkig.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgufenzy.top/gtnglaixab.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gthjojrnhx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yongpay.top/gtabibbcbn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.bjfxy.top/gthbbjwzjy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtghuodyab.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydzc1.top/gtohhllbsl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhengqikj.top/gtvyfhoxbv.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtbrliybln.html

Py:   s.splitlines()
来源：http://hz.wangshuangyany.cn/gtrqrwfanh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtrsgsnxtx.html

JS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtbobwrjvf.html

TS:   s.split(/\r?\n/)
来源：http://hz.daxiang520.top/gttwvfvadw.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gtsmatdkcq.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxinkj.top/gtmevikoph.html

Ruby: s.lines
来源：http://hz.meibo888.top/gtlrkrgeky.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtcqpmnleu.html

[E20] 判断字符串是否为空
来源：http://hz.jiagoushi.top/gtiriuhnbq.html

Py:   if not s:
来源：http://hz.chenjidiqi.icu/gtiuifyirb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sweek.top/gtilvkxbxx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sysykeji.top/gtncfvmtfj.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtdmfxvsai.html

Java: if (s.isEmpty()) {}
来源：http://hz.daxiang520.top/gtwwstoegq.html

Go:   if s == "" {}
来源：http://hz.smart0.xyz/gtwdwwrlbm.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtrbbbpxhc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.feifeiyinyue.top/gtyuyzdryb.html

[E21] 超长截断加省略号
来源：http://hz.ehwqpu.com/gtbdomgihn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ehwqpu.com/gtyqenowjb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtqolnmlxt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtbaqzyzcq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtvxcubfll.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtllotqmgs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhengqikj.top/gtlskxjaum.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gttudxowfm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtugjoodyt.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtrlljqlor.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtbkbwgchp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtfksfgrki.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtjbqttfhz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jinqigfzy.top/gtsgvdlorz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cheryme.top/gteqgrkcqf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangshuangyany.cn/gtjhhcsmbt.html

Ruby: s.bytesize;  s.length
来源：http://hz.quarkkingdee.top/gtulvtjhrp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hongshengwenyu.top/gtindfdqcd.html

================================================================================
来源：http://hz.yj202588.top/gtykzmgabq.html

F. 文件与目录
来源：http://hz.yangfankeji.com/gtjbdowjvf.html

================================================================================
来源：http://hz.wangdashe.top/gtyhnsgicx.html

[F01] 读取整个文件
来源：http://hz.dianchejie.cn/gtvhtivtea.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tanke756.top/gtrodbvswu.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhixingplan.top/gtqbikknea.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cashguo.top/gtkbvmaxlt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.daxiang520.top/gtwfrbvlpz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.guannengcc.top/gtabxrsvbm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtthrzovtq.html

Ruby: File.read("a.txt")
来源：http://hz.52xcode.cn/gtaublgppw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jyoumei.cn/gtkgwcyyfr.html

[F02] 逐行读取文件
来源：http://hz.havefunace.top/gtrnhqpeik.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gttsfrupzd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.cucudq.cn/gtibyfsphn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.andypj.xyz/gtzdfjuiwn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.svipenyu.cn/gtesqqixec.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yueranfly.top/gtsbeygidd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtosaijmtm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhaomingkeji.xyz/gtgmwehdjk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtxfjypfvi.html

[F03] 写入文件（覆盖）
来源：http://hz.zdqjudy.top/gtzhzdbacu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinyuanbaomall.cn/gtabvcaalf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.bjfxy.top/gtqygiphjb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gthibfrbjb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtmldpygey.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gogol.net.cn/gtrprmyxyq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhengqikj.top/gtwpbxumgr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gttvmsvcbr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtsbunrvxp.html

[F04] 追加写入文件
来源：http://hz.wangshuangyany.cn/gtyuosfuuc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinqigfzy.top/gtgiqfsyxk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.0kj1m.cn/gtocxeevxr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jiagoushi.top/gtjpcszhep.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtixcawojc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sweek.top/gtarqkgjma.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.pengpengdd.cyou/gtcxxcsqiu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hywenlv.cn/gtftcydxuf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jinyuanbaomall.cn/gtdhgdsyxz.html

[F05] 判断文件或目录是否存在
来源：http://hz.shzxlz.cn/gtznbeqzgd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yuanzhike.top/gtupwvyujg.html

PHP:  file_exists("a.txt");
来源：http://hz.9152youxi.cn/gtaveczjww.html

JS:   fs.existsSync("a.txt")
来源：http://hz.cucudq.cn/gtqvzkyaqb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yonumen.top/gtivwhuysr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtdcuigmjp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtmirwripw.html

Ruby: File.exist?("a.txt")
来源：http://hz.haohaochexian.top/gtavwmfysc.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gteuwucbyb.html

[F06] 删除文件
来源：http://hz.meibo888.top/gtrhxwwrlb.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtsnjfqnma.html

PHP:  unlink("a.txt");
来源：http://hz.ydjk.org.cn/gtpxahytud.html


<!-- 参考信息 -->