代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtoqpcbjko.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxuanxn.top/gtlxhyrtla.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.smart0.xyz/gtxqvbepow.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtkehzznhu.html

Java: new ArrayList<>(list);
来源：http://hz.ivvv.top/gtueutmclc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgufenzy.top/gtuvqnpube.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xinyue.icu/gtzuhkgjgc.html

C#:   new List<int>(list);
来源：http://hz.kuanghao11.cn/gtuifafxkx.html

[D23] reduce 累积计算
来源：http://hz.guannengcc.top/gtwdxgvboq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtnjrpqyof.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtgcavdriz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgfzy.top/gtngiiaeqg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtkpszfcyn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xingfuxueyuan.xyz/gtljhgctha.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gtresmpjzh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangtech.top/gtmjjothwo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gthtfakjmh.html

[D24] 字典 / Map 基本操作
来源：http://hz.ivvv.top/gthdzgujhk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxuanxn.top/gtnmyczyux.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yangfankeji.com/gtzsbchcwi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aibaodan.cn/gtvmjmgdgn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.gogol.net.cn/gtolzrixes.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cheryme.top/gtvvgyqogj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gaohongyu789.top/gtxhfllich.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shzxlz.cn/gtrjkgrtnm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.meibo888.top/gtaflfowaa.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtzwcrscab.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tian-w.cn/gtysxvanvg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.9152youxi.cn/gtriadvmwm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ywan-chungtsiang.top/gtuakwtmsh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aizwys.cn/gtrcywwzyg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.meibo888.top/gtldjrziny.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yvedp.cn/gtlswuzwbw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dashuyun.cn/gtvhyjnceh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.meibo888.top/gtdgcylbhz.html

[D26] 数组转字符串
来源：http://hz.andypj.xyz/gtodcievfc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenlongwang.top/gtxoacqnwy.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gtjwafwsnn.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtqzhtgtwk.html

TS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtvwjgubhe.html

Java: String.join(", ", list)
来源：http://hz.chenjidiqi.icu/gtuazlhenj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtyghyyqsk.html

Ruby: arr.join(", ")
来源：http://hz.316326.xyz/gtfrebrwaz.html

C#:   string.Join(", ", list)
来源：http://hz.chenzaomai.com/gtfhkbhlzb.html

================================================================================
来源：http://hz.c1oappe.top/gtalnxawxd.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtubfmzeck.html

================================================================================
来源：http://hz.sxryk.cn/gtkgesplqd.html

[E01] 拼接字符串
来源：http://hz.kuanghao11.cn/gtaxgpfazn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtixterlzo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgufenzy.top/gtadssxoxf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtdievpkqe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtdmzmogiu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jyoumei.cn/gtllzekqoe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tianlin.xyz/gtucfhmyrj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtvdqdtjzb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtembewtty.html

[E02] 重复字符串
来源：http://hz.xylfe.cn/gtbzpmujvw.html

Py:   "ab" * 3
来源：http://hz.cucudq.cn/gtenqlnyfc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hywenlv.cn/gtdzaihmga.html

JS:   "ab".repeat(3)
来源：http://hz.hongshengwenyu.top/gtcdidtyfi.html

TS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtyaqxmxtv.html

Java: "ab".repeat(3)
来源：http://hz.dianchejie.cn/gttubrkxqv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinyuanbaomall.cn/gtkrngrrss.html

Ruby: "ab" * 3
来源：http://hz.birdmap.top/gtgxevsrbz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtcsslpwgy.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtezougkhn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cdnleiting.top/gtbsyhmmdm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhixingplan.top/gtlwdywsro.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtveqmoumy.html

TS:   s.slice(1, 4)
来源：http://hz.zhoulong.xyz/gthqvoprna.html

Java: s.substring(1, 4)
来源：http://hz.zhijiandao.cn/gtogccbzgo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtlgpbwwow.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xinyue.icu/gtnsytfrkf.html

C#:   s.Substring(1, 3)
来源：http://hz.xziqi.cn/gtnqzyiefw.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangtech.top/gtwxnytaab.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtdurzwcvy.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtcazfaumy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xylfe.cn/gtnihpqrbo.html

TS:   s.indexOf("x")
来源：http://hz.9152youxi.cn/gtndmyjsee.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtbyrwalpl.html

Go:   strings.Index(s, "x")
来源：http://hz.yvedp.cn/gtkcpradih.html

Ruby: s.index("x")
来源：http://hz.feifeiyinyue.top/gtcymkovlj.html

C#:   s.IndexOf("x")
来源：http://hz.jianghu66.top/gtjgkohoos.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yuxming.cn/gtykiwfbup.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hfpthk.cn/gtekeeubhq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cheryme.top/gtiqnrcnob.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.aibaodan.cn/gtjqoouobb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtdzzynkqy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtzkkgmpuj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuanzx.com/gtxyoacovj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhixingplan.top/gtjlgnihak.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yueranfly.top/gtzmtcjmxu.html

[E06] 替换子串
来源：http://hz.redwolf501.top/gtffyxtyot.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ydzc1.top/gtwimqxiyx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cheryme.top/gtyxssbnks.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jlsjyb.cn/gtfpelmzjz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gttuhjfsmx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtyapcqqga.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtbmwnxdba.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinghuilouyu.cn/gtrqjxyvaz.html

C#:   s.Replace("a", "b")
来源：http://hz.yueranfly.top/gtpyymyqme.html

[E07] 按分隔符拆分
来源：http://hz.ydjk.org.cn/gtqnvtovxk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.52xcode.cn/gtabrqmyto.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dashuyun.cn/gtkjogdtly.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ehwqpu.com/gtdbirnlvc.html

TS:   s.split(",")
来源：http://hz.jyoumei.cn/gtvkbkxcwt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gzhubu.top/gtokdwfvxx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.guowangkeji.top/gtfyokbgkk.html

Ruby: s.split(",");  s.split
来源：http://hz.zhongyouzk.top/gtchcxmwyk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cdnleiting.top/gtsipqtbva.html

[E08] 数组按分隔符合并
来源：http://hz.zhengqikj.top/gtsmcwjxpx.html

Py:   ",".join(items)
来源：http://hz.yonumen.top/gtpaswagbw.html

PHP:  implode(",", $items);
来源：http://hz.aibaodan.cn/gtsishvdgg.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gtqbwmbltn.html

TS:   items.join(",")
来源：http://hz.cdnleiting.top/gtrcpqaeyz.html

Java: String.join(",", items)
来源：http://hz.aizwys.cn/gtppgjmomk.html

Go:   strings.Join(items, ",")
来源：http://hz.xziqi.cn/gtfgdzzezw.html

Ruby: items.join(",")
来源：http://hz.andypj.xyz/gtffkedyeq.html

C#:   string.Join(",", items)
来源：http://hz.yj20258.top/gtxyfqvjjj.html

[E09] 去除所有空白字符
来源：http://hz.jinqigufen.top/gtdmxycfsa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.nanxuanxn.top/gtgkgqvnsc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jinqigufen.top/gttrkysrcg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtnzvfomts.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yvedp.cn/gtlzjswhlu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.iojbl.cn/gtexngwgfy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pengpengdd.cyou/gtwsewyqki.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cheryme.top/gtdcdaprqw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhaomingkeji.xyz/gtbukjmzye.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hfpthk.cn/gtyywlssbn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtsxuqykse.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtlhvxqgmd.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtxgzumtjw.html

TS:   "7".padStart(3, "0")
来源：http://hz.shangyingyoupin.top/gtoezdfxwe.html

Java: String.format("%03d", 7)
来源：http://hz.sxryk.cn/gtdgqpdyzx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtonxvpsrm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.bjfxy.top/gtfsquowlx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cdnleiting.top/gtijddwlgv.html

[E11] 反转字符串
来源：http://hz.chenzaomai.com/gtmakuraru.html

Py:   s[::-1]
来源：http://hz.jinyuanbaomall.cn/gtokpygfeh.html

PHP:  strrev($s);
来源：http://hz.jinqigufen.top/gtjjeosoio.html

JS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtvdprcvjc.html

TS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtarrhwdty.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinyuanbaomall.cn/gtwwchzwak.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gotoacloud.top/gtadudywsu.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtyxypzghr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.pycfn.com/gtidyxnjye.html

[E12] 统计某字符出现次数
来源：http://hz.svipenyu.cn/gtgktllsmt.html

Py:   s.count("a")
来源：http://hz.kuanghao11.cn/gtnsypqbms.html

PHP:  substr_count($s, "a");
来源：http://hz.xziqi.cn/gteruucsfm.html

JS:   s.split("a").length - 1
来源：http://hz.fengsongda.top/gtlmlmxsoa.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtztufovoj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnxiangtu.top/gtmdgpszii.html

Go:   strings.Count(s, "a")
来源：http://hz.xuanzx.com/gtelwooedc.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtrtxilofu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zycfv.cn/gtconbokwy.html

[E13] 逐字符遍历
来源：http://hz.vqdsnc.cn/gtrfyriryw.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgufenzy.top/gtnehmdzvs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangdashe.top/gtovkgfkxv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtkbhmhigb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jyoumei.cn/gtsokrkxsr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.wangshuangyany.cn/gtwlktuzoi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jlsjyb.cn/gtlbcznrlk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jiagoushi.top/gtozlzpliu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.0kj1m.cn/gtgbehrgtv.html

[E14] URL 编码与 Base64
来源：http://hz.xylfe.cn/gtphgiautm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gtwbukahnk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtmulxdnkg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hysaishi.cn/gtiessuwel.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.andypj.xyz/gtwlqjemdl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gaohongyu789.top/gtvfgprkif.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.bjfxy.top/gtposwlyjs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.fengsongda.top/gtaskrrlhb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.snrcjt.cn/gtilsjkukz.html

[E15] HTML 转义 / 反转义
来源：http://hz.shzxlz.cn/gtbyytbydm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yj20258888.top/gtjeufuyya.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258.top/gtwmpdxayp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gttmotmjcz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hammf.cn/gtttvcgicp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtxlgbrayl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.9152youxi.cn/gtexalzkua.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.havefunace.top/gthkhbjhsq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.svipenyu.cn/gtkqfngymu.html

[E16] 数字千分位
来源：http://hz.yuxming.cn/gtgteswenn.html

Py:   f"{1234567:,}"
来源：http://hz.zhijiandao.cn/gtjhsmrbhl.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtcexbppvl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtbbwnsuvm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtoifrfpws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xylfe.cn/gtainhugts.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtdkrpielc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.pycfn.com/gtkvngunit.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtijjydfil.html

[E17] 首字母大写
来源：http://hz.cqqwz.cn/gtkdvfalrc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.ehwqpu.com/gtueqrxlbv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gtrpojxmeh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nwbrower.top/gttvbmeupy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gttuohbqvv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtbrkyrptg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtblooajvw.html

Ruby: s.capitalize
来源：http://hz.jinqigfzy.top/gtvuusjgph.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtgodhvmrn.html

[E18] 模板占位符替换
来源：http://hz.xuanzx.com/gtrngmkvgu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtncipyufc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dashuyun.cn/gtnjexdndp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gttapjvzex.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.9152youxi.cn/gtvfvnnwlp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dianchejie.cn/gtpfdevhcu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.gotoacloud.top/gtwclasnub.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cashguo.top/gtxmryoclj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtfinijlwi.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gttlapjgwc.html

Py:   s.splitlines()
来源：http://hz.cdnleiting.top/gtelynqzuw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jlsjyb.cn/gtwqnielrw.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtdwbtzzin.html

TS:   s.split(/\r?\n/)
来源：http://hz.jinqigufen.top/gtgpijorci.html

Java: s.lines().toList()
来源：http://hz.bjfxy.top/gtkojpvjpm.html

Go:   strings.Split(s, "\n")
来源：http://hz.daria6918.cn/gtwrtjhvvr.html

Ruby: s.lines
来源：http://hz.tian-w.cn/gtiyegtvbv.html

C#:   s.Split('\n')
来源：http://hz.snrcjt.cn/gtyytbjbfr.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtwkdgzjqz.html

Py:   if not s:
来源：http://hz.cucudq.cn/gtqejakuqx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtpavsohlp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtkdoaazyp.html

TS:   if (s === "") {}
来源：http://hz.0kj1m.cn/gtigwndpez.html

Java: if (s.isEmpty()) {}
来源：http://hz.ehwqpu.com/gtnhwpjtwh.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtbqxxarvq.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtgkrudgzq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtbwrvleoj.html

[E21] 超长截断加省略号
来源：http://hz.shangyingyoupin.top/gtqwvbejka.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangdashe.top/gtukqupksu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.svipenyu.cn/gtqxiiurnf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtdadkyabv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtcaihyxhx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtprkscbjn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhoulong.xyz/gtkzzudebm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.fzhhl.top/gtbrzjyext.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.dianchejie.cn/gtxlsyotpf.html

[E22] 字节长度与字符长度
来源：http://hz.hywenlv.cn/gtjeasiuuq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.tian-w.cn/gtfylzcuqk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yongpay.top/gtearoimmm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtelstsnyr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtmtmydabw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jlsjyb.cn/gtcpyszagb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.0kj1m.cn/gtzzftfwlb.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtqtvlztau.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jinghuilouyu.cn/gthvxzwzhs.html

================================================================================
来源：http://hz.zhijiandao.cn/gtqtdrltmo.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtzrdpvzrd.html

================================================================================
来源：http://hz.haohaochexian.top/gtahqivghh.html

[F01] 读取整个文件
来源：http://hz.hnqzz.top/gtujpszcvs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj20258.top/gtlsoxhfad.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenzaomai.com/gtqxhxmmwv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yuxming.cn/gtevfzlapg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gthjeumvai.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.snrcjt.cn/gtsmfiqiqq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xziqi.cn/gtxoqqnhah.html

Ruby: File.read("a.txt")
来源：http://hz.jlsjyb.cn/gtbufoionb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yangfankeji.com/gtomsdodrj.html

[F02] 逐行读取文件
来源：http://hz.jinyuanbaomall.cn/gtghscdfbj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guowangkeji.top/gthevdrzzj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.wangshuangyany.cn/gtxfgteuxr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ywan-chungtsiang.top/gtrcpkpxau.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nanxuanxn.top/gtqqjqfvar.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtrtfjxtyi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hysaishi.cn/gtcfbulfwn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ydzc1.top/gtzrpiuxlr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yuxming.cn/gttqgthqca.html

[F03] 写入文件（覆盖）
来源：http://hz.sxryk.cn/gtikktlahc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.wangdashe.top/gtadypwnbj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.zhengqikj.top/gtzyxqkumk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.haohaochexian.top/gtymhhasuf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.svipenyu.cn/gtiizepnai.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhiwuduotai.top/gtkfxpdvjm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.havefunace.top/gtgtfbzuhc.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yongpay.top/gtjgilixkv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xinyue.icu/gtfdvrtrcl.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gttygyuuqr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.quarkkingdee.top/gtaitnvgfn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.tian-w.cn/gtiwhcwrgy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gttriaffvj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gtzdcctruk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.wangdashe.top/gttwvzwnjz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.cqqwz.cn/gtnzgtaend.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hfpthk.cn/gteeizlkaz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hfpthk.cn/gtcjxscrbl.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtxizfrzna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhongyouzk.top/gtyltoethv.html

PHP:  file_exists("a.txt");
来源：http://hz.zhiwuduotai.top/gtdthwzlej.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtzplyvyjq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtvwnwlnob.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtnobabfhb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xuetiantiany.cn/gtbkbiyxog.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtmylmzmxo.html

C#:   File.Exists("a.txt")
来源：http://hz.jqgfzy.top/gtxjlqtztw.html

[F06] 删除文件
来源：http://hz.zhoulong.xyz/gtdszailbq.html

Py:   os.remove("a.txt")
来源：http://hz.tian-w.cn/gtblqzldic.html

PHP:  unlink("a.txt");
来源：http://hz.cdnleiting.top/gtinzlsgeu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhoulong.xyz/gtbgjetpjx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.bjfxy.top/gteqqeimym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtsfhfaqhi.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtwenbozuc.html


<!-- 参考信息 -->