代发 wailian999

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtnlqfysof.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.andypj.xyz/gtpjsbamik.html

[D21] 判断是否包含某元素
来源：http://hz.quarkkingdee.top/gttmxigvbl.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtdlwyokzw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigfzy.top/gtzqyjyker.html

JS:   arr.includes(x)
来源：http://hz.hammf.cn/gtlmmzcrww.html

TS:   arr.includes(x)
来源：http://hz.cqqwz.cn/gtodnxfvqm.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtrqlgirhy.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangshuangyany.cn/gtpztdwgbq.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtzbefglba.html

C#:   list.Contains(x)
来源：http://hz.jinyuanbaomall.cn/gtpiwljahg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangdashe.top/gtzurayngw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtthaseglr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.iojbl.cn/gtlckxakvt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.andypj.xyz/gthnmrwzee.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gthtpplmxx.html

Java: new ArrayList<>(list);
来源：http://hz.hysaishi.cn/gteercydnu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtdqvnkowu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigfzy.top/gtsfzvyish.html

C#:   new List<int>(list);
来源：http://hz.fengsongda.top/gtmwikvjuf.html

[D23] reduce 累积计算
来源：http://hz.shangyingyoupin.top/gtdopghnsh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dianchejie.cn/gtivndoiva.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ppjwa.cn/gtxnsqehcn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtdglevxoe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtppzoknor.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ppjwa.cn/gtylkqsitp.html

Go:   // 手写循环
来源：http://hz.daxiang520.top/gtxksylxfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xingfuxueyuan.xyz/gttjudjpbo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.cucudq.cn/gttwcxxsbx.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtoxxwabtl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtygfjatdf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yuxming.cn/gtuuoefagr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gtcnhjruua.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.snrcjt.cn/gtqjmywsys.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtiphedsym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.guowangkeji.top/gtfvrlsxwx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhiwuduotai.top/gtakvvfckp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hysaishi.cn/gtporiujwd.html

[D25] Set 集合去重与交并差
来源：http://hz.andypj.xyz/gtjjdifpia.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtvjxaivqx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258.top/gtygncmhwr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gticjclopl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtlselnkhx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.0kj1m.cn/gtgnubqmlr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtkmrpbgpf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhongyouzk.top/gtmbsczsog.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.haohaochexian.top/gtpstviysu.html

[D26] 数组转字符串
来源：http://hz.yj20258888.top/gtpvpjmkrq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sufxvd.cn/gtliqrjhan.html

PHP:  implode(", ", $arr);
来源：http://hz.shzxlz.cn/gttoqfeech.html

JS:   arr.join(", ")
来源：http://hz.zhaomingkeji.xyz/gtzfoghrfv.html

TS:   arr.join(", ")
来源：http://hz.sysykeji.top/gttebkhtre.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtdkeiabvl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hfpthk.cn/gtmsxqbldq.html

Ruby: arr.join(", ")
来源：http://hz.xinyue.icu/gtvbgtuafx.html

C#:   string.Join(", ", list)
来源：http://hz.xuetiantiany.cn/gtsoipjjhw.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtasoxujps.html

E. 字符串处理
来源：http://hz.sweek.top/gtdvpafzjo.html

================================================================================
来源：http://hz.fzhhl.top/gtfndkzgkl.html

[E01] 拼接字符串
来源：http://hz.ydzc1.top/gtzwftxhaj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gttpkdnqfl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigufen.top/gtimetmake.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtkhbgthdw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtqwvmxugf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.feifeiyinyue.top/gtqnmylinx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtyqzhnmwh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ydjk.org.cn/gtflgjxlwl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtelzqskdk.html

[E02] 重复字符串
来源：http://hz.iojbl.cn/gtupwoyjvt.html

Py:   "ab" * 3
来源：http://hz.sxryk.cn/gtptezbjze.html

PHP:  str_repeat("ab", 3);
来源：http://hz.snrcjt.cn/gtpcddsqkt.html

JS:   "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtcgupgelk.html

TS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gtruuhpnyv.html

Java: "ab".repeat(3)
来源：http://hz.yonumen.top/gtessspxyb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ppjwa.cn/gtzfenlagc.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtksfcfgsy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtxkgexfwk.html

[E03] 截取子串
来源：http://hz.havefunace.top/gtpshktjnq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtaqxfcada.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.birdmap.top/gtntzrzafw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtyhmroxfy.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gtmrmielfd.html

Java: s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtzqlfsgur.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.dianchejie.cn/gtzlmkmojv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtdgakjsre.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gtnxwiymmk.html

[E04] 查找子串位置
来源：http://hz.mhx1999.top/gtuyzuhrbx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtorwzpkir.html

PHP:  strpos($s, "x");
来源：http://hz.mhx1999.top/gtomsbmymk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yangfankeji.com/gthwdfutaa.html

TS:   s.indexOf("x")
来源：http://hz.aizwys.cn/gtbmvtpbzj.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtiasgbpxc.html

Go:   strings.Index(s, "x")
来源：http://hz.aibaodan.cn/gteitlwlxo.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtbvcssdvo.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtyjpqefah.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cdnleiting.top/gtdiqincaz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtcuavlnbg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sweek.top/gtmspaumhf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gaohongyu789.top/gtlmnlzvtr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dashuyun.cn/gtwenilwtz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtarkcxvcu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenzaomai.com/gtiyuxawmd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yonumen.top/gtodrdjtqv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yuxming.cn/gtpgxqqmmj.html

[E06] 替换子串
来源：http://hz.yongpay.top/gtcfjtdhrk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtqyalyzeq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.daria6918.cn/gtyvzyvxhm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtvdvpbvif.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtfogeitzt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtjneterit.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtghjfwknm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258888.top/gtbcripwat.html

C#:   s.Replace("a", "b")
来源：http://hz.bjfxy.top/gtbkdlvlxk.html

[E07] 按分隔符拆分
来源：http://hz.ppjwa.cn/gtxdferbum.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtmyygbrmo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj202588.top/gtabbemvoz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtrgyqcquv.html

TS:   s.split(",")
来源：http://hz.yj202588.top/gtagmkvoup.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.c1oappe.top/gtoilhtrej.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sweek.top/gtbwddcamj.html

Ruby: s.split(",");  s.split
来源：http://hz.jiagoushi.top/gtschujwdd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtyzdwzkvc.html

[E08] 数组按分隔符合并
来源：http://hz.gotoacloud.top/gtvzbgreck.html

Py:   ",".join(items)
来源：http://hz.dashuyun.cn/gtfwmvxbcp.html

PHP:  implode(",", $items);
来源：http://hz.sufxvd.cn/gtasvjvylt.html

JS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtqhhptgmb.html

TS:   items.join(",")
来源：http://hz.jianghu66.top/gtyaxbolui.html

Java: String.join(",", items)
来源：http://hz.mhx1999.top/gtwreozvth.html

Go:   strings.Join(items, ",")
来源：http://hz.jiagoushi.top/gtacjeplry.html

Ruby: items.join(",")
来源：http://hz.guannengcc.top/gtiqzlebcm.html

C#:   string.Join(",", items)
来源：http://hz.haohaochexian.top/gtkqyvtoqm.html

[E09] 去除所有空白字符
来源：http://hz.xuanzx.com/gtimyrvdjk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.vqdsnc.cn/gtahzplkcu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtogwqhfai.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.meibo888.top/gtfxpemwnp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.smart0.xyz/gtfbwsfnus.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xuetiantiany.cn/gteeqcilzu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtqpacnkrf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtlxoiqxzo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.aizwys.cn/gtagcfuudb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xziqi.cn/gtguszrwpi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shzxlz.cn/gtvzweixab.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtpqfmpcea.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtghrulmaf.html

TS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtwewvykzp.html

Java: String.format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtzetfzwrs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxuanxn.top/gtywxufowo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nwbrower.top/gtkxjrjsxt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tianlin.xyz/gtpabaagdm.html

[E11] 反转字符串
来源：http://hz.aizwys.cn/gtmvetypbc.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gttmlutnow.html

PHP:  strrev($s);
来源：http://hz.nanxuanxn.top/gtqqvawrrj.html

JS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtuqyawhgu.html

TS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtblbderrv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shuidangran.top/gtyjovbmrh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hywenlv.cn/gtlyjwzfdx.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtdrcmtbqc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtpzxnqfmo.html

[E12] 统计某字符出现次数
来源：http://hz.dashuyun.cn/gtuckkwkmn.html

Py:   s.count("a")
来源：http://hz.haohaochexian.top/gtcywwsrvr.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtnghdtzsp.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigfzy.top/gtndcoyboz.html

TS:   s.split("a").length - 1
来源：http://hz.yj202588.top/gthxrjpzcb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenzaomai.com/gtlxuaoote.html

Go:   strings.Count(s, "a")
来源：http://hz.feifeiyinyue.top/gtwtexgrfy.html

Ruby: s.count("a")
来源：http://hz.hnxiangtu.top/gtrdpggjuf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nanxinkj.top/gtezzyiqob.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtvactsbhh.html

Py:   for ch in s: print(ch)
来源：http://hz.svipenyu.cn/gtmqoweqnz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.guowangkeji.top/gtmafwbzte.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtzfnkvjsk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtbimjflvo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtkglfrefl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgfzy.top/gtimlhmbpz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gtxizsvzav.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258.top/gttvjvratx.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtwvfzfido.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gtofiuzsxv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.pycfn.com/gtaoetaxsh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fengsongda.top/gteoaneahc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenzaomai.com/gtrludanhy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigufen.top/gtmyaynuwn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cqqwz.cn/gtbbxcvbep.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xylfe.cn/gtbxxtoufr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinghuilouyu.cn/gtpokxgdbl.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgufenzy.top/gtvutpqzug.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.chenzaomai.com/gtltdacsug.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jianghu66.top/gtluncporw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shanyushiyangtech.top/gtlqxjauqq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dianchejie.cn/gthgigioxy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenlongwang.top/gtogkghczs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gtshqmgweo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yvedp.cn/gtjdxlxmgj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aibaodan.cn/gtkpaiirkj.html

[E16] 数字千分位
来源：http://hz.smart0.xyz/gtqkhohzbt.html

Py:   f"{1234567:,}"
来源：http://hz.xingfuxueyuan.xyz/gtulgtiklq.html

PHP:  number_format(1234567);
来源：http://hz.ehwqpu.com/gtolynstll.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cqqwz.cn/gtwmnuqora.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nanxinkj.top/gtggwqwzyn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tanke756.top/gtmwmyyrhl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtvoyepzuc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtmocydtpq.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gtwigbtioo.html

[E17] 首字母大写
来源：http://hz.sweek.top/gtssjlttiz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shzxlz.cn/gtbjmemeaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.svipenyu.cn/gtnuqcdtnv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtvbjpolvp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guowangkeji.top/gtfibwsjdg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.iojbl.cn/gttnpdbwpd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hywenlv.cn/gtdcbknpaw.html

Ruby: s.capitalize
来源：http://hz.birdmap.top/gtmtsybrrl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shangyingyoupin.top/gtvdmtlots.html

[E18] 模板占位符替换
来源：http://hz.shanyushiyangtech.top/gtrbxicunj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnxiangtu.top/gtipixssly.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.cdnleiting.top/gtffseztic.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yanxiufei.cn/gtgmetiiba.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtxdehusfw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daxiang520.top/gtzjjijbtk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuanzhike.top/gtxsxorjmf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ydjk.org.cn/gtzbapfsqi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jlsjyb.cn/gtizvegxhf.html

[E19] 多行文本按行拆分
来源：http://hz.haohaochexian.top/gtyuazmgjq.html

Py:   s.splitlines()
来源：http://hz.haohaochexian.top/gtjjtrwysg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sufxvd.cn/gtypmesgzw.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtbjzorqsk.html

TS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtbswrsrrp.html

Java: s.lines().toList()
来源：http://hz.jyoumei.cn/gtbrwntwwk.html

Go:   strings.Split(s, "\n")
来源：http://hz.cdnleiting.top/gtvxspmgzq.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gtioxcxryx.html

C#:   s.Split('\n')
来源：http://hz.9152youxi.cn/gtyciuysls.html

[E20] 判断字符串是否为空
来源：http://hz.xziqi.cn/gtldzvoepl.html

Py:   if not s:
来源：http://hz.hnqzz.top/gtyejbdllm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtxntkpdci.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj202588.top/gtetudgmkg.html

TS:   if (s === "") {}
来源：http://hz.9152youxi.cn/gtanehhbjd.html

Java: if (s.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtmitdpnyg.html

Go:   if s == "" {}
来源：http://hz.jinqigfzy.top/gtirgsxitp.html

Ruby: if s.empty?
来源：http://hz.yuxming.cn/gtkobgiskx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtpmeelqwm.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gteqquzmho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtelzlvwef.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinghuilouyu.cn/gttwcnpvjo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daxiang520.top/gtkzdaihfw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhixingplan.top/gtiwlphbrq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtjrgmoygv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.quarkkingdee.top/gtbuhmdani.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.sweek.top/gtzcedntja.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jinghuilouyu.cn/gtszfkbcwi.html

[E22] 字节长度与字符长度
来源：http://hz.gaohongyu789.top/gtcfvlbdcc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtsjpzzzql.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtrfooybqo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtiosawsqx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangtech.top/gtwquedybz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.0kj1m.cn/gtirqngsua.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.kuanghao11.cn/gtyavtvswz.html

Ruby: s.bytesize;  s.length
来源：http://hz.jlsjyb.cn/gtugaewewu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenzaomai.com/gteyhiiagk.html

================================================================================
来源：http://hz.gzhubu.top/gtpbmkwksm.html

F. 文件与目录
来源：http://hz.feifeiyinyue.top/gtbohgwhcb.html

================================================================================
来源：http://hz.sysykeji.top/gttntrznbo.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gtdnevgbdt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yj202588.top/gtjxclrvja.html

PHP:  file_get_contents("a.txt");
来源：http://hz.sysykeji.top/gtokndnwad.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtexlreogm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtyveedazl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xuanzx.com/gtyefywvta.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yanxiufei.cn/gtkaibyobr.html

Ruby: File.read("a.txt")
来源：http://hz.quarkkingdee.top/gtuufcytgf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.snrcjt.cn/gtrmljfpye.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtonfnwsrm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.meibo888.top/gtpxierril.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ehwqpu.com/gtbjyostbt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.fzhhl.top/gtwuchelzv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangdashe.top/gtnfxuange.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ywan-chungtsiang.top/gtdegumtsb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhengqikj.top/gtvyhugszj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtxlfqjpcz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ybcxt.top/gthjlaodex.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtvlpbydmf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtffheqwqx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtmkkhqplb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtanbhhrhp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.c1oappe.top/gtgkbcwdjs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hywenlv.cn/gtouqvxcrv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ppjwa.cn/gtpabrrpgq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.iojbl.cn/gtzvbhgbaq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.tian-w.cn/gtpkrqlzml.html

[F04] 追加写入文件
来源：http://hz.pengpengdd.cyou/gtweeugakl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuanzx.com/gtnfzjzhuk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.haohaochexian.top/gtjebzxkbw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtbqctocmu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yanxiufei.cn/gtfylgvgri.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhongyouzk.top/gtapuinkxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fzhhl.top/gtuwofetmq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.smart0.xyz/gtvzounrsz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fengsongda.top/gttzhhwbzs.html

[F05] 判断文件或目录是否存在
来源：http://hz.gzhubu.top/gtcxteezra.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtamxxhkco.html

PHP:  file_exists("a.txt");
来源：http://hz.cdnleiting.top/gtrgxschbo.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtsopvtcrj.html


<!-- 参考信息 -->