代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yanxiufei.cn/gtedilwzgb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.vqdsnc.cn/gteerolymr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xziqi.cn/gtmqszxieg.html

TS:   [...arr];
来源：http://hz.cucudq.cn/gtnelnifvr.html

Java: new ArrayList<>(list);
来源：http://hz.havefunace.top/gtdakkihir.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtiqgqwfwe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtchdqlgxf.html

C#:   new List<int>(list);
来源：http://hz.sweek.top/gtdvjxwfhp.html

[D23] reduce 累积计算
来源：http://hz.yj20258888.top/gtwotlbygn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtxvmibsdh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtqpocxwnm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtrqcaiajg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gtjxedrtue.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuetiantiany.cn/gtdnfaureu.html

Go:   // 手写循环
来源：http://hz.gogol.net.cn/gtfbawxlqx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gtlrdqaxbg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yangfankeji.com/gtmnngswuk.html

[D24] 字典 / Map 基本操作
来源：http://hz.sweek.top/gtqhlztdsw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yonumen.top/gtqnxxnsdu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gthwtecbji.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hammf.cn/gtgqqatoum.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shangyingyoupin.top/gtlikjwsht.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtfdjjdubw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuanzhike.top/gtpoztdaiv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jqgufenzy.top/gtmzgtnjvf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydjk.org.cn/gtfvacssqg.html

[D25] Set 集合去重与交并差
来源：http://hz.hongshengwenyu.top/gtbniusxwm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinqigfzy.top/gteldgaiqm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.9152youxi.cn/gtapdbxwsm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dashuyun.cn/gtthmtmfyg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.kuanghao11.cn/gtbldpurco.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtdidzdtou.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtomakyjdi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shuidangran.top/gtzlufllat.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gtpwaqanuo.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtvolwwgnq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.birdmap.top/gtzewdybci.html

PHP:  implode(", ", $arr);
来源：http://hz.jinqigufen.top/gtuspiwkso.html

JS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gtyhjfbstl.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtwzfyxyec.html

Java: String.join(", ", list)
来源：http://hz.andypj.xyz/gtsdndacid.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ehwqpu.com/gtqwhlhkhc.html

Ruby: arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtmjczwvcw.html

C#:   string.Join(", ", list)
来源：http://hz.316326.xyz/gtiyogkffs.html

================================================================================
来源：http://hz.ydzc1.top/gtcipqilzn.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtfburubwz.html

================================================================================
来源：http://hz.iojbl.cn/gtgvlkltel.html

[E01] 拼接字符串
来源：http://hz.yj202588.top/gtcbfokbvx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtaoqrflij.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sxryk.cn/gtgmagzjov.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtpzdounwc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxuanxn.top/gtzgsdvtfn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yongpay.top/gtojfactgs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gotoacloud.top/gtqnismjky.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtsdqimiwu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tanke756.top/gthmfmoewk.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gtmbuoxipx.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtwvvefjet.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tanke756.top/gtlxknwxjm.html

JS:   "ab".repeat(3)
来源：http://hz.tanke756.top/gtsmbxqzgx.html

TS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtqmzuisqc.html

Java: "ab".repeat(3)
来源：http://hz.ydzc1.top/gtcxxkpywj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtrqjukbry.html

Ruby: "ab" * 3
来源：http://hz.pengpengdd.cyou/gtazcspkzp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgfzy.top/gtjaefseuu.html

[E03] 截取子串
来源：http://hz.aibaodan.cn/gtulrvwzhc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jlsjyb.cn/gtyvubxzey.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtrgvrsfiq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtpipfljlk.html

TS:   s.slice(1, 4)
来源：http://hz.tanke756.top/gtliywxarb.html

Java: s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtvhsfcylc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ywan-chungtsiang.top/gtcebrrxqh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.mhx1999.top/gtwoqyimai.html

C#:   s.Substring(1, 3)
来源：http://hz.xinyue.icu/gtvvhydbue.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangtech.top/gtygvltxei.html

Py:   s.find("x");  s.index("x")
来源：http://hz.havefunace.top/gtzbipsdzc.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gthaccmxsi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtpomocphv.html

TS:   s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtxdygifpu.html

Java: s.indexOf("x")
来源：http://hz.daria6918.cn/gtoeecdiwt.html

Go:   strings.Index(s, "x")
来源：http://hz.guannengcc.top/gtlqfwxbeo.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gtyqpisnad.html

C#:   s.IndexOf("x")
来源：http://hz.yongpay.top/gtktfureip.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhongyouzk.top/gtwdujqfin.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fzhhl.top/gtnvvvuiyw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tian-w.cn/gtewnaedsw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtqotftvyk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.aibaodan.cn/gtncexvkey.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.redwolf501.top/gtgdgsegor.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.meibo888.top/gtpsvtxihu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gtxwxbjwdx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhijiandao.cn/gtzgxeujoc.html

[E06] 替换子串
来源：http://hz.xziqi.cn/gtkuakiplt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhijiandao.cn/gtuifkjbfy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.snrcjt.cn/gtbhfqbgya.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinghuilouyu.cn/gtxnsscdmz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.chenjidiqi.icu/gtbufgasxh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gotoacloud.top/gtujeiehzp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shanyushiyangkeji.top/gtrxqearho.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtohzlqcuf.html

C#:   s.Replace("a", "b")
来源：http://hz.yonumen.top/gtyoiskaez.html

[E07] 按分隔符拆分
来源：http://hz.yanxiufei.cn/gtxwarcpoo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xingfuxueyuan.xyz/gttrphmfhb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gtmnffdvgk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hysaishi.cn/gthgmjxqlp.html

TS:   s.split(",")
来源：http://hz.yonumen.top/gtwjwlydlw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.guannengcc.top/gtconiydzj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gthcxxujqx.html

Ruby: s.split(",");  s.split
来源：http://hz.bjfxy.top/gtufbymwss.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtfwiajdpz.html

[E08] 数组按分隔符合并
来源：http://hz.svipenyu.cn/gtokadiccz.html

Py:   ",".join(items)
来源：http://hz.zhaomingkeji.xyz/gtplbxmnzf.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gthepirczi.html

JS:   items.join(",")
来源：http://hz.nanxinkj.top/gtzdifrxwx.html

TS:   items.join(",")
来源：http://hz.hysaishi.cn/gtjtzowczm.html

Java: String.join(",", items)
来源：http://hz.gotoacloud.top/gtvxasdzdh.html

Go:   strings.Join(items, ",")
来源：http://hz.ybcxt.top/gtkvrroxnv.html

Ruby: items.join(",")
来源：http://hz.redwolf501.top/gthehkhxqd.html

C#:   string.Join(",", items)
来源：http://hz.jqgufenzy.top/gtlhlywoyb.html

[E09] 去除所有空白字符
来源：http://hz.cashguo.top/gthkxxiumh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhoulong.xyz/gtazgekzzz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj20258.top/gtxpvpsaui.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtsqyugisa.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtifufkbsz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtylidbcca.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yongpay.top/gtaijmzyyg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinqigfzy.top/gtwomhppso.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtjzxmlnok.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj20258.top/gtnooylkym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cashguo.top/gtnllbhqmu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangtech.top/gtssozjxiw.html

JS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtveeeaamf.html

TS:   "7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtllhrccot.html

Java: String.format("%03d", 7)
来源：http://hz.tanke756.top/gtlqotmigw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dashuyun.cn/gtkpszmntl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtbdewwmik.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yangfankeji.com/gtcqyvsqhx.html

[E11] 反转字符串
来源：http://hz.dianchejie.cn/gtphtbnrcd.html

Py:   s[::-1]
来源：http://hz.sxryk.cn/gtlvsnpxov.html

PHP:  strrev($s);
来源：http://hz.yj20258.top/gtzxjcfgjv.html

JS:   [...s].reverse().join("")
来源：http://hz.andypj.xyz/gtidggcgnt.html

TS:   [...s].reverse().join("")
来源：http://hz.zhongyouzk.top/gtvcfryqqh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dianchejie.cn/gtxoghlbbx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sxryk.cn/gtkoricdzo.html

Ruby: s.reverse
来源：http://hz.zhengqikj.top/gtxfwtkwsr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gotoacloud.top/gtbuhnmkyz.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtqhllxkky.html

Py:   s.count("a")
来源：http://hz.feifeiyinyue.top/gtpmebmxwl.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtldtxrbqv.html

JS:   s.split("a").length - 1
来源：http://hz.yueranfly.top/gtoyyurwuq.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtjshjlcpd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.andypj.xyz/gtzcziunfm.html

Go:   strings.Count(s, "a")
来源：http://hz.yvedp.cn/gtnjcvmvuj.html

Ruby: s.count("a")
来源：http://hz.cqqwz.cn/gtjovmklof.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cheryme.top/gtwsdigmsh.html

[E13] 逐字符遍历
来源：http://hz.sweek.top/gtaqnccaah.html

Py:   for ch in s: print(ch)
来源：http://hz.yvedp.cn/gtryacuqbl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jyoumei.cn/gtnwektdwp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtprdcgglt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtprfiatwb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuetiantiany.cn/gthvlyrfbg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gthgewjqta.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigufen.top/gthxsdbqeh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtpydnvigq.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gtaegnlywx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jyoumei.cn/gtoahnwaid.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtykicordj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangshuangyany.cn/gtvvoulodx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.andypj.xyz/gtcvhunjzk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgfzy.top/gtgmuyrafb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pycfn.com/gtpmdqvbjs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtiptlrqct.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtjhkskzvo.html

[E15] HTML 转义 / 反转义
来源：http://hz.fzhhl.top/gtamfqkauf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtpfhwmpur.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gttcycfius.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhijiandao.cn/gtdafgbvnw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jinyuanbaomall.cn/gtwfopzvjx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gtazhjrkbx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gthjdoxppi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.pycfn.com/gtcggbqnnz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guowangkeji.top/gtqwntprpi.html

[E16] 数字千分位
来源：http://hz.nanxinkj.top/gtwekiwosl.html

Py:   f"{1234567:,}"
来源：http://hz.yuanzhike.top/gtqqfouwqq.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gttlyavlpy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtktbuesfw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jyoumei.cn/gtkdnhjwro.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xingfuxueyuan.xyz/gtuvmwvhyx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtnzwrzawl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhengqikj.top/gtpnergdqx.html

C#:   1234567.ToString("N0")
来源：http://hz.ydzc1.top/gtrqlgzxep.html

[E17] 首字母大写
来源：http://hz.fengsongda.top/gtegguudcp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shzxlz.cn/gtztgmonim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtnubvlytf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtmblrmfzr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtkazgecxc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hysaishi.cn/gthhjefbxj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuxming.cn/gtgxsfqger.html

Ruby: s.capitalize
来源：http://hz.yuxming.cn/gtjalxbvhk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.andypj.xyz/gtehbvunvd.html

[E18] 模板占位符替换
来源：http://hz.kuanghao11.cn/gtiksxdaaa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtnbwwgeux.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hongshengwenyu.top/gtmudgtsle.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtwhkgeibg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yonumen.top/gtqclwmbji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtvchhbahl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.chenjidiqi.icu/gtfpzbcklr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtkmdqffmt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.fengsongda.top/gtimzhhwyl.html

[E19] 多行文本按行拆分
来源：http://hz.yanxiufei.cn/gthcsuwdpw.html

Py:   s.splitlines()
来源：http://hz.ybcxt.top/gtysjsyqra.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtefaxddtk.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gttivgdiyy.html

TS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtsecyjvjj.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtycykiepa.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtrqawjgqc.html

Ruby: s.lines
来源：http://hz.jinqigufen.top/gtdydjqtgy.html

C#:   s.Split('\n')
来源：http://hz.quarkkingdee.top/gtoftpmand.html

[E20] 判断字符串是否为空
来源：http://hz.yvedp.cn/gtnjsnrymg.html

Py:   if not s:
来源：http://hz.ivvv.top/gtolpuuxqc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxinkj.top/gtdamgpskx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gtgptgvcbv.html

TS:   if (s === "") {}
来源：http://hz.hnqzz.top/gtdqelldvl.html

Java: if (s.isEmpty()) {}
来源：http://hz.shuidangran.top/gtvgqretkx.html

Go:   if s == "" {}
来源：http://hz.xuanzx.com/gtjpzrfqxs.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtmwktemot.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ivvv.top/gtnfarprnx.html

[E21] 超长截断加省略号
来源：http://hz.jiagoushi.top/gtjcwulhjs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cqqwz.cn/gtbcmyftlv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinyuanbaomall.cn/gtktmtgoth.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtejtziqgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtjbuzdcrp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtavjimaql.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtnswcufbc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtudxxzoao.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtxcxzwebt.html

[E22] 字节长度与字符长度
来源：http://hz.sysykeji.top/gthiskbwbq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ydjk.org.cn/gttgsctcxy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cdnleiting.top/gtlhjdboos.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtqargccbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtwpmrgsdv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gogol.net.cn/gtafryuken.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhengqikj.top/gtchgyparp.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangkeji.top/gtuwollhrc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.wangdashe.top/gtqeqlgayr.html

================================================================================
来源：http://hz.shzxlz.cn/gtzofcfdew.html

F. 文件与目录
来源：http://hz.nanxinkj.top/gtohjytobm.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtosnlesar.html

[F01] 读取整个文件
来源：http://hz.9152youxi.cn/gtspkhtufz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangdashe.top/gtrlmrpafo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxuanxn.top/gtiltcihtl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jiagoushi.top/gtdmlzbazb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yanxiufei.cn/gtuqeqbnsu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtadbreowo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtvwpzupet.html

Ruby: File.read("a.txt")
来源：http://hz.bjfxy.top/gttohfvvqm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangtech.top/gtanabvfov.html

[F02] 逐行读取文件
来源：http://hz.feifeiyinyue.top/gtlajtspua.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.fzhhl.top/gtkqlibsvt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.aibaodan.cn/gtcbpcwlly.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtrzqnvpgq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fengsongda.top/gtaszpzpve.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtdimrtmtx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.pycfn.com/gttvqrrgxr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nanxuanxn.top/gtvosxxqft.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.wangdashe.top/gtjwpsxyxq.html

[F03] 写入文件（覆盖）
来源：http://hz.yangfankeji.com/gttpbgeqsj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gttnhcruxi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtprkutapb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtfjfjokkt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtmuogxext.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yongpay.top/gtuhmdsayh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.gzhubu.top/gtejcsbwfq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhaomingkeji.xyz/gtfakkbuyg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.andypj.xyz/gtkgwbmitf.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtkoyqjxly.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtjofsrlaw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtpoplxdgy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.haohaochexian.top/gtwwgkwkcu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtaoujmzsw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.ywan-chungtsiang.top/gtplbdpqhn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nwbrower.top/gtlkgknwov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuetiantiany.cn/gtifdfeqgk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtuarmirok.html

[F05] 判断文件或目录是否存在
来源：http://hz.cqqwz.cn/gtzoubpabu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ybcxt.top/gtjmovvzkw.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtziafxkhk.html

JS:   fs.existsSync("a.txt")
来源：http://hz.zhongyouzk.top/gtwozryggb.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gthikyuooo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xinyue.icu/gtgyaxktyx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.chenjidiqi.icu/gtxutyptme.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangshuangyany.cn/gtxvwzxkbv.html

C#:   File.Exists("a.txt")
来源：http://hz.ywan-chungtsiang.top/gttlqnhowd.html

[F06] 删除文件
来源：http://hz.jinghuilouyu.cn/gtizlfuior.html

Py:   os.remove("a.txt")
来源：http://hz.fzhhl.top/gtemgzpwod.html

PHP:  unlink("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtpzqfyxav.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtzudsuvna.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ivvv.top/gtfcksnxqa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtfcxcbric.html

Go:   os.Remove("a.txt")
来源：http://hz.redwolf501.top/gttvwlheek.html


<!-- 参考信息 -->