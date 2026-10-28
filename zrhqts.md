代发 wailian999

[D23] reduce 累积计算
来源：http://hz.yongpay.top/gtbbimpkhl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtgjhmnrbn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tianlin.xyz/gtewgmjfry.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtrcspiglq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtgifxmzxc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangshuangyany.cn/gtdqrukfks.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtanicyqup.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gogol.net.cn/gtgzkkltld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cashguo.top/gtzxsmdbyr.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxinkj.top/gtxnmzcbgh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtmsttxilr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtmxumdcci.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.0kj1m.cn/gtjcbwqbfy.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhiwuduotai.top/gteujrhurh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gotoacloud.top/gtvljtduag.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtamufimbc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gtmapevdwx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sufxvd.cn/gtsxuzeqtt.html

[D25] Set 集合去重与交并差
来源：http://hz.feifeiyinyue.top/gtgnnqmtye.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gttfmgicda.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gtvjxiajjt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtjxkzweke.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuanzx.com/gtyrltfbfn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtvquxakrc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gthdvdpsrc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinqigfzy.top/gtkejbnyra.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shuidangran.top/gtnqqpmoln.html

[D26] 数组转字符串
来源：http://hz.cheryme.top/gtwumlyaxj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.andypj.xyz/gtalakflxl.html

PHP:  implode(", ", $arr);
来源：http://hz.sufxvd.cn/gtwbitxptp.html

JS:   arr.join(", ")
来源：http://hz.tian-w.cn/gthaelhqjt.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtjehzhkkk.html

Java: String.join(", ", list)
来源：http://hz.zhiwuduotai.top/gtoghaegtb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtlhsthfbb.html

Ruby: arr.join(", ")
来源：http://hz.yj202588.top/gtbotcgell.html

C#:   string.Join(", ", list)
来源：http://hz.jinghuilouyu.cn/gtazmtkjos.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtnwlrrfco.html

E. 字符串处理
来源：http://hz.hfpthk.cn/gtkramsxsv.html

================================================================================
来源：http://hz.gogol.net.cn/gtvolqbqjp.html

[E01] 拼接字符串
来源：http://hz.tianlin.xyz/gtxjfwwklz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtshazrgrl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangshuangyany.cn/gtzvqeeptv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtqyuyfmbo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtmiemnagu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhoulong.xyz/gtlktpknzn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ybcxt.top/gtmrllzqvy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.redwolf501.top/gtgnsfagjk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.c1oappe.top/gterzeviwm.html

[E02] 重复字符串
来源：http://hz.sxryk.cn/gtwfwbhekb.html

Py:   "ab" * 3
来源：http://hz.jinghuilouyu.cn/gtgjtkjlny.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnqzz.top/gtlsmghwiy.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtepftdvjj.html

TS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtqfikvgwv.html

Java: "ab".repeat(3)
来源：http://hz.zhixingplan.top/gtscpdvcdu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gtolnnmcxt.html

Ruby: "ab" * 3
来源：http://hz.yonumen.top/gtnlluxnzt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.birdmap.top/gtrvgofxvi.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gtfnfotbez.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtcvhadjby.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.mhx1999.top/gtsemnzawg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtdkypfbym.html

TS:   s.slice(1, 4)
来源：http://hz.c1oappe.top/gthbmtrdfz.html

Java: s.substring(1, 4)
来源：http://hz.sysykeji.top/gtgqhhbirz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daria6918.cn/gtljlxxulu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hammf.cn/gtxrkjrizo.html

C#:   s.Substring(1, 3)
来源：http://hz.dashuyun.cn/gtcafojvqg.html

[E04] 查找子串位置
来源：http://hz.fzhhl.top/gtxvwccsfy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinghuilouyu.cn/gttsvidcqz.html

PHP:  strpos($s, "x");
来源：http://hz.zhoulong.xyz/gtqpkxthye.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gtttfucjaq.html

TS:   s.indexOf("x")
来源：http://hz.ydzc1.top/gtxufqwxgk.html

Java: s.indexOf("x")
来源：http://hz.cashguo.top/gtyrqxxdkq.html

Go:   strings.Index(s, "x")
来源：http://hz.jinqigufen.top/gtlfbsomte.html

Ruby: s.index("x")
来源：http://hz.chenjidiqi.icu/gtasdkalhj.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtzdypeprj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gtrgjjxmev.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cqqwz.cn/gtmeshvick.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydjk.org.cn/gtruarahie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtsjdyfqyo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenlongwang.top/gtlrglkenz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtfkavqmti.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yangfankeji.com/gtbppydjfv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenjidiqi.icu/gtfwkfoonm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgufenzy.top/gtsfrwfwmu.html

[E06] 替换子串
来源：http://hz.nanxuanxn.top/gtwuqvyrig.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jianghu66.top/gtbmlafqak.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenlongwang.top/gthfqjdeos.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtjdziaobe.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtlvaritoc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtjauhkckk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtramroedb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gtgbfrscvi.html

C#:   s.Replace("a", "b")
来源：http://hz.zhixingplan.top/gtjsjhbksr.html

[E07] 按分隔符拆分
来源：http://hz.yvedp.cn/gtcmmfdwlt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gogol.net.cn/gtczocrjdw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.birdmap.top/gthiiazklb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shzxlz.cn/gtykdlsosu.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtzyrfprpw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.haohaochexian.top/gtxsnoyjno.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tianlin.xyz/gtjwcydnjp.html

Ruby: s.split(",");  s.split
来源：http://hz.zhixingplan.top/gteecutxyx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gthzdtlypb.html

[E08] 数组按分隔符合并
来源：http://hz.cqqwz.cn/gtffjvocyv.html

Py:   ",".join(items)
来源：http://hz.pengpengdd.cyou/gtyzrvrrno.html

PHP:  implode(",", $items);
来源：http://hz.chenlongwang.top/gtpbyhyyts.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtddgbadtu.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtpzylyomu.html

Java: String.join(",", items)
来源：http://hz.gzhubu.top/gtchnpjquj.html

Go:   strings.Join(items, ",")
来源：http://hz.sweek.top/gtwtzgtrnp.html

Ruby: items.join(",")
来源：http://hz.cucudq.cn/gtypsztsfg.html

C#:   string.Join(",", items)
来源：http://hz.dianchejie.cn/gtqoigbuyp.html

[E09] 去除所有空白字符
来源：http://hz.redwolf501.top/gtjxvyyvkd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dashuyun.cn/gttjsfsilw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtqcjpicng.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hammf.cn/gtwapnmdrl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtydldadco.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jlsjyb.cn/gtrdtgthqs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hfpthk.cn/gtfkohokty.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sxryk.cn/gtoqugzqjo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtkdaewsij.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tian-w.cn/gtsalmrxem.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtubjfjxsb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.meibo888.top/gtmhnrczur.html

JS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtcbbjswpf.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtzcphvgju.html

Java: String.format("%03d", 7)
来源：http://hz.andypj.xyz/gtzowvamfb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtbrjnkhkw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.mhx1999.top/gtwoujhefm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenzaomai.com/gtvibmcqjj.html

[E11] 反转字符串
来源：http://hz.jlsjyb.cn/gtcnycfrek.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtjzsfxoro.html

PHP:  strrev($s);
来源：http://hz.quarkkingdee.top/gttomhcwtg.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtfdqvucbg.html

TS:   [...s].reverse().join("")
来源：http://hz.yuanzhike.top/gtxdibhziz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fzhhl.top/gtkvgrhyoq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.c1oappe.top/gtmoiknxpm.html

Ruby: s.reverse
来源：http://hz.aibaodan.cn/gtspgjlfug.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtkjwzejta.html

[E12] 统计某字符出现次数
来源：http://hz.vqdsnc.cn/gtmccbhyrx.html

Py:   s.count("a")
来源：http://hz.jinqigufen.top/gtawwjkilo.html

PHP:  substr_count($s, "a");
来源：http://hz.ehwqpu.com/gtlcaliztq.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtagcxfkqe.html

TS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtjjoopbpv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtboavjjyc.html

Go:   strings.Count(s, "a")
来源：http://hz.yuanzhike.top/gthowukzbb.html

Ruby: s.count("a")
来源：http://hz.yj20258.top/gtpjovanyb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.vqdsnc.cn/gtrpdhgqnw.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtvzspyweb.html

Py:   for ch in s: print(ch)
来源：http://hz.iojbl.cn/gtnipbphsw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ivvv.top/gtzkqfxjnk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhijiandao.cn/gtyarrfxfp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtmhclohzx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shzxlz.cn/gtthyvelft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fzhhl.top/gtabepjrgc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fengsongda.top/gtllhgtpsi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtebxuypin.html

[E14] URL 编码与 Base64
来源：http://hz.feifeiyinyue.top/gtmkdbvxml.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.daria6918.cn/gttouhkalv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenjidiqi.icu/gtmhcpmxyw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aibaodan.cn/gtdhdnwowq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtdopvdkra.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.sysykeji.top/gtbdkcipkl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangdashe.top/gtwqaiozbr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yanxiufei.cn/gtdotcksne.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hfpthk.cn/gtacvqwvlw.html

[E15] HTML 转义 / 反转义
来源：http://hz.vqdsnc.cn/gtcvlgvufs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenlongwang.top/gtzmekkoiv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.daxiang520.top/gtbzqyikdx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tanke756.top/gtzlquxhgt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xinyue.icu/gthapjdret.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuanzhike.top/gtgozvubnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gtbrmqjckd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.smart0.xyz/gtoregvqyg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.kuanghao11.cn/gtyvjofcbv.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtwfjuyrdd.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gtbpwrtmgk.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gttaqqikaq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtrkctjzpo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtfpcpsaiw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ybcxt.top/gtnbmagxxb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.shanyushiyangtech.top/gtfsanjotd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sxryk.cn/gtlbustavp.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtqxlkjmaa.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtpcdmjwro.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shzxlz.cn/gtxxkzgfam.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ydzc1.top/gtbbitbtjl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtflpjqupq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtjnkvcobx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ehwqpu.com/gtzxpfzoku.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jyoumei.cn/gtdwgrbrdp.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtqpavwwop.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.smart0.xyz/gtjuwtwjwp.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangtech.top/gtekdozxri.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ivvv.top/gttxszswzp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jlsjyb.cn/gtprdliqyo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtxmjfmtea.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtssdkheiy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.chenzaomai.com/gtktgbabfc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.snrcjt.cn/gtddxajqca.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gtkxcdlyxa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hongshengwenyu.top/gtvoqpqnxj.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtnzxzonbl.html

Py:   s.splitlines()
来源：http://hz.shzxlz.cn/gteyqzjncw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.fzhhl.top/gtrmhqsari.html

JS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gtdwoyslrh.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtypvjqzdx.html

Java: s.lines().toList()
来源：http://hz.0kj1m.cn/gtnlvcaxzx.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinghuilouyu.cn/gtzoeamjxo.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtloxlyjzk.html

C#:   s.Split('\n')
来源：http://hz.xingfuxueyuan.xyz/gtnxytsnnm.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gthymfgmrs.html

Py:   if not s:
来源：http://hz.sweek.top/gtaxlrefvr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenlongwang.top/gtmsropfaf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhixingplan.top/gtesvixwbg.html

TS:   if (s === "") {}
来源：http://hz.jinyuanbaomall.cn/gtbqujrlls.html

Java: if (s.isEmpty()) {}
来源：http://hz.havefunace.top/gtlezwcgmk.html

Go:   if s == "" {}
来源：http://hz.zhijiandao.cn/gtjdqcnkbp.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtgxlgfola.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xinyue.icu/gtupekmcbh.html

[E21] 超长截断加省略号
来源：http://hz.xylfe.cn/gtgwupafgg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtdipwmufw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.0kj1m.cn/gtsogsovno.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gthnixzzrl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtzfrseiiu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtypivtwsb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhongyouzk.top/gtjnixtrfj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aibaodan.cn/gtiaxiljfj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtionukonr.html

[E22] 字节长度与字符长度
来源：http://hz.cucudq.cn/gtcbheelmk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fengsongda.top/gtamzjdgfu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuanzhike.top/gtydxcjiiq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ivvv.top/gtviviotco.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.tianlin.xyz/gtbbflvdbd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yongpay.top/gtfvmpyzkl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gtzurlgsno.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenlongwang.top/gtxfqrrhlc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gzhubu.top/gtewnuavjc.html

================================================================================
来源：http://hz.52xcode.cn/gtugvvnvuu.html

F. 文件与目录
来源：http://hz.wangdashe.top/gtebpyynhd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtytafsjrv.html

[F01] 读取整个文件
来源：http://hz.zdqjudy.top/gtdyqrxyle.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtzeyrbcqz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinghuilouyu.cn/gtfivtxisu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gthgczsoby.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hywenlv.cn/gtydrtdqzk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtljbngjeo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zdqjudy.top/gtjoqeuboz.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtwomdcraf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhengqikj.top/gtsfofidtc.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtczucmmhd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.smart0.xyz/gtkhhtjdgn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shanyushiyangkeji.top/gtowthroji.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cucudq.cn/gtwffzmomy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shanyushiyangkeji.top/gtjcboojpt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cqqwz.cn/gtlhhtdqqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gtdqccsrtv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtzesmhgld.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtxvyzicdn.html

[F03] 写入文件（覆盖）
来源：http://hz.yangfankeji.com/gtdjalzjvk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigufen.top/gtrcfvunnb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj20258.top/gtvwlxodlf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtvxnaorjc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hfpthk.cn/gtkqgwxnzc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sweek.top/gtrrihhlkg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yongpay.top/gtkwowslyr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.wangshuangyany.cn/gttzjwtefb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtbilgahok.html

[F04] 追加写入文件
来源：http://hz.kuanghao11.cn/gtiimesppx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtdhokxohn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.iojbl.cn/gtgalcbrej.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jlsjyb.cn/gtjyzfmatu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jinqigfzy.top/gtfcxpapba.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhoulong.xyz/gtwynzyitt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gtipnfakzo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydzc1.top/gtkemhsmya.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhongyouzk.top/gtrjgijquk.html

[F05] 判断文件或目录是否存在
来源：http://hz.yueranfly.top/gthnqkbeep.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.chenjidiqi.icu/gttrtxkxyh.html

PHP:  file_exists("a.txt");
来源：http://hz.hnqzz.top/gtptlazycg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtjwhzgowl.html

TS:   fs.existsSync("a.txt")
来源：http://hz.wangshuangyany.cn/gtrppnjagk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtehtbiamj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtbpojmaet.html

Ruby: File.exist?("a.txt")
来源：http://hz.xuetiantiany.cn/gtatmiahgf.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtvjwksqbh.html

[F06] 删除文件
来源：http://hz.shanyushiyangkeji.top/gteljopnrd.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtaokmtzvn.html

PHP:  unlink("a.txt");
来源：http://hz.chenzaomai.com/gtotuascav.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtogxrlbym.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtsfqnnipz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtaywewupg.html

Go:   os.Remove("a.txt")
来源：http://hz.nanxuanxn.top/gtrfdahpdy.html

Ruby: File.delete("a.txt")
来源：http://hz.316326.xyz/gtzajeealm.html

C#:   File.Delete("a.txt");
来源：http://hz.ydzc1.top/gtqfgpespu.html

[F07] 创建目录（含多级）
来源：http://hz.ydzc1.top/gtabgsutza.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.snrcjt.cn/gtvaranppy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtohlkkbqt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtkrfzfadc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.daxiang520.top/gtuqpmzvol.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtvfodmjsw.html


<!-- 参考信息 -->