代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jianghu66.top/gterrkhhmf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ehwqpu.com/gtyqoswhuu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhoulong.xyz/gtvupdssdr.html

TS:   [...arr];
来源：http://hz.chenlongwang.top/gthqwcwove.html

Java: new ArrayList<>(list);
来源：http://hz.kuanghao11.cn/gtphfuzzcy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.pycfn.com/gtmonxspgv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.daria6918.cn/gtdrdugykm.html

C#:   new List<int>(list);
来源：http://hz.nanxinkj.top/gtxxkjotlu.html

[D23] reduce 累积计算
来源：http://hz.yanxiufei.cn/gtlqwxbxqa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtetazmjzx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gtitvzbivy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtpraffmai.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtogllseyl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gtiemuqbqa.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtbdprobps.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yonumen.top/gtqwckvfsq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.feifeiyinyue.top/gtvdftxsga.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigfzy.top/gtdhsfxxpf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fengsongda.top/gtmiaimrkr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhaomingkeji.xyz/gtqxcnkjsi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jlsjyb.cn/gtpgxwwexu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtzdzihrqq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtyplfrwuu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zycfv.cn/gtbjixqjnx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.316326.xyz/gtqncmfqxd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtlmvbmqik.html

[D25] Set 集合去重与交并差
来源：http://hz.guowangkeji.top/gtpgcptwdx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtepwhcotc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhaomingkeji.xyz/gtdbyahpej.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtkjcgcrjp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zycfv.cn/gttaklaump.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.snrcjt.cn/gtnqqfrwsg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ppjwa.cn/gthaswipjo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnqzz.top/gtwsldhcrb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258888.top/gtavvshfmp.html

[D26] 数组转字符串
来源：http://hz.daxiang520.top/gtvhkkppyz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtrzbvzcqz.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxinkj.top/gtmfivqreu.html

JS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtnepisjbk.html

TS:   arr.join(", ")
来源：http://hz.hfpthk.cn/gttfofcmvb.html

Java: String.join(", ", list)
来源：http://hz.xuetiantiany.cn/gtdsfandoe.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtgetnhxzt.html

Ruby: arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtqudkqlik.html

C#:   string.Join(", ", list)
来源：http://hz.yj202588.top/gtmtlsjsts.html

================================================================================
来源：http://hz.cqqwz.cn/gtbahvbbxf.html

E. 字符串处理
来源：http://hz.zhixingplan.top/gtzvwymzzi.html

================================================================================
来源：http://hz.wangdashe.top/gtwooinmkv.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gthphatnkh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jyoumei.cn/gtdwttolwx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj202588.top/gtyrvkzipw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtnbabqkff.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtnufuyiev.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hfpthk.cn/gtmcivisqi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtjcyotkqy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gtspawdwtj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinghuilouyu.cn/gtekgddgfr.html

[E02] 重复字符串
来源：http://hz.mhx1999.top/gtfgdjktvb.html

Py:   "ab" * 3
来源：http://hz.haohaochexian.top/gtdjcumgjr.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtgrloiaud.html

JS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtkabyjzny.html

TS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtjvnodprp.html

Java: "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtippbbqys.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtremyfsit.html

Ruby: "ab" * 3
来源：http://hz.quarkkingdee.top/gtakcjkenb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtoxznpgxc.html

[E03] 截取子串
来源：http://hz.jinqigufen.top/gtvhyvfoqk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj20258.top/gtlmwqqnwf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenjidiqi.icu/gtzkjbjoyd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xingfuxueyuan.xyz/gtgwyhyqos.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtnyqmcpny.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gttuxrfaki.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtnplhekti.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangshuangyany.cn/gtnlshpeed.html

C#:   s.Substring(1, 3)
来源：http://hz.sweek.top/gtfutoomzh.html

[E04] 查找子串位置
来源：http://hz.zhijiandao.cn/gtsvxunfed.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhoulong.xyz/gtgiorjqiu.html

PHP:  strpos($s, "x");
来源：http://hz.zhongyouzk.top/gtnbjiujlx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenlongwang.top/gtszepmyrz.html

TS:   s.indexOf("x")
来源：http://hz.xuanzx.com/gtdzznantc.html

Java: s.indexOf("x")
来源：http://hz.dashuyun.cn/gtiseuiacd.html

Go:   strings.Index(s, "x")
来源：http://hz.zhixingplan.top/gthziswycf.html

Ruby: s.index("x")
来源：http://hz.jlsjyb.cn/gtiofupyye.html

C#:   s.IndexOf("x")
来源：http://hz.havefunace.top/gtexnslhwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhoulong.xyz/gtpkdsqnhp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gtcrsjgbxh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.haohaochexian.top/gtnniswrbo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtnpphlauc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.pengpengdd.cyou/gtwyuoixzu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxinkj.top/gtoxqwtnze.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jyoumei.cn/gtsvxcnohy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pengpengdd.cyou/gtedxejkip.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtxhyyslgt.html

[E06] 替换子串
来源：http://hz.havefunace.top/gthhddgvwn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gttfujwrqo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jiagoushi.top/gttjtmaozb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nwbrower.top/gtptfhxyzx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gthmacwuva.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gogol.net.cn/gtjxtmrpzc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.wangdashe.top/gtdhjsadic.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tanke756.top/gtkldevjgd.html

C#:   s.Replace("a", "b")
来源：http://hz.zhiwuduotai.top/gtfjhkxxjh.html

[E07] 按分隔符拆分
来源：http://hz.havefunace.top/gtpgznwphu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtyopyycav.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtfqzbhglz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hnqzz.top/gtufpjkfav.html

TS:   s.split(",")
来源：http://hz.chenlongwang.top/gtspleixpp.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gtibnfptto.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.snrcjt.cn/gtrtoqrksb.html

Ruby: s.split(",");  s.split
来源：http://hz.sysykeji.top/gthtcnvqqh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtankmvjju.html

[E08] 数组按分隔符合并
来源：http://hz.xinyue.icu/gtbinhkfug.html

Py:   ",".join(items)
来源：http://hz.bjfxy.top/gtalkxdpmj.html

PHP:  implode(",", $items);
来源：http://hz.zhiwuduotai.top/gtqskibxmv.html

JS:   items.join(",")
来源：http://hz.nwbrower.top/gtmesiejqc.html

TS:   items.join(",")
来源：http://hz.ydjk.org.cn/gtxlcodjwv.html

Java: String.join(",", items)
来源：http://hz.pengpengdd.cyou/gtdlsaauio.html

Go:   strings.Join(items, ",")
来源：http://hz.daria6918.cn/gttcnuyyls.html

Ruby: items.join(",")
来源：http://hz.yuxming.cn/gtakcycyvo.html

C#:   string.Join(",", items)
来源：http://hz.jlsjyb.cn/gtynedmvww.html

[E09] 去除所有空白字符
来源：http://hz.nanxinkj.top/gtwbdoaoyc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.andypj.xyz/gtxiqrgusj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.guowangkeji.top/gtglcfaomj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtolcmczmm.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtxzwwvpwo.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gtqpooxeeg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.9152youxi.cn/gtfyotxuiq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.daria6918.cn/gtgydbbzmn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gtbvdgpkpy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.kuanghao11.cn/gtkwkgcjsu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.haohaochexian.top/gtbrcyzpck.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shangyingyoupin.top/gtkcxfnfzh.html

JS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtesngybit.html

TS:   "7".padStart(3, "0")
来源：http://hz.hnqzz.top/gttyjmgdky.html

Java: String.format("%03d", 7)
来源：http://hz.guannengcc.top/gtlbtcmipp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtoiqhctdl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258888.top/gtaeamnfym.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.52xcode.cn/gtktqfzydz.html

[E11] 反转字符串
来源：http://hz.tanke756.top/gtnlqrfxcf.html

Py:   s[::-1]
来源：http://hz.zhongyouzk.top/gtggzsuupq.html

PHP:  strrev($s);
来源：http://hz.tian-w.cn/gttyrfvnqm.html

JS:   [...s].reverse().join("")
来源：http://hz.quarkkingdee.top/gtkbrviqtz.html

TS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtlphdnbhz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuanzhike.top/gtwrtzhmnu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtefhlahdh.html

Ruby: s.reverse
来源：http://hz.shanyushiyangtech.top/gtqujdwiha.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.haohaochexian.top/gtdkkkyrij.html

[E12] 统计某字符出现次数
来源：http://hz.xinyue.icu/gtpycbbajn.html

Py:   s.count("a")
来源：http://hz.shuidangran.top/gteolebhls.html

PHP:  substr_count($s, "a");
来源：http://hz.birdmap.top/gtwqzsoodx.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtfvnvnsba.html

TS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtnhepgrca.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xingfuxueyuan.xyz/gtvbrvligx.html

Go:   strings.Count(s, "a")
来源：http://hz.hywenlv.cn/gtwcmglbad.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gthcibjybh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtglpydmpx.html

[E13] 逐字符遍历
来源：http://hz.wangdashe.top/gtjvqyiekx.html

Py:   for ch in s: print(ch)
来源：http://hz.xingfuxueyuan.xyz/gtpypfqufb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hongshengwenyu.top/gtewypbfoj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtkdvmbpyb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cheryme.top/gtynhosehj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtvsyfxtqk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sxryk.cn/gtomjceksu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuanzx.com/gtjzgwhmky.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shzxlz.cn/gthubvnssv.html

[E14] URL 编码与 Base64
来源：http://hz.aibaodan.cn/gtyevpctjp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sxryk.cn/gtedpljyyw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtnnzckgkn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuxming.cn/gtvdrnfqcu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cucudq.cn/gtglnhrzjb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtzdysvbpl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cdnleiting.top/gtatfyepmt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jianghu66.top/gtfyhfzhkv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtxlbqyewf.html

[E15] HTML 转义 / 反转义
来源：http://hz.yuanzhike.top/gtzcnoyosb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhengqikj.top/gtlfvbxepb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zycfv.cn/gtptfvgeeb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.wangdashe.top/gtcrmguglp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhaomingkeji.xyz/gtzjluwswk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gogol.net.cn/gtwofswwoh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuanzx.com/gtmutguicq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cheryme.top/gtygellulj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhoulong.xyz/gtlnkfwrzs.html

[E16] 数字千分位
来源：http://hz.mhx1999.top/gtnofmmovg.html

Py:   f"{1234567:,}"
来源：http://hz.cashguo.top/gtdiulukcg.html

PHP:  number_format(1234567);
来源：http://hz.zhiwuduotai.top/gtvlxtlpvi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtnjqmcxcw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gttsgddfcz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yonumen.top/gtnctjbyqm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtzczfyocq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ivvv.top/gtkssdyzxi.html

C#:   1234567.ToString("N0")
来源：http://hz.9152youxi.cn/gtmekjcqrm.html

[E17] 首字母大写
来源：http://hz.wangdashe.top/gteknrpsjs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhijiandao.cn/gthaebxeeb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.gotoacloud.top/gtertxofur.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtynpnpxry.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtzarjjrrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.wangshuangyany.cn/gtlctrjlbq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xinyue.icu/gtctbcbbnn.html

Ruby: s.capitalize
来源：http://hz.bjfxy.top/gtytuczshz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.wangshuangyany.cn/gtullhyryb.html

[E18] 模板占位符替换
来源：http://hz.tanke756.top/gtfkvxzoad.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtirbcfcyy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhaomingkeji.xyz/gtpotyggyq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.fzhhl.top/gtzqyirqzt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydjk.org.cn/gtpcsjxjlo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fzhhl.top/gtvknnddbt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guowangkeji.top/gtjguxczxv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gzhubu.top/gtqwupequk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.gotoacloud.top/gtqtwycnxi.html

[E19] 多行文本按行拆分
来源：http://hz.dashuyun.cn/gtmyhanhpi.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtohntfsrd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.0kj1m.cn/gthwgpvmwe.html

JS:   s.split(/\r?\n/)
来源：http://hz.wangshuangyany.cn/gthywxngzd.html

TS:   s.split(/\r?\n/)
来源：http://hz.pycfn.com/gtoohigxir.html

Java: s.lines().toList()
来源：http://hz.c1oappe.top/gtzsxnezma.html

Go:   strings.Split(s, "\n")
来源：http://hz.shzxlz.cn/gtnprfluzm.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtsmyhxfnh.html

C#:   s.Split('\n')
来源：http://hz.kuanghao11.cn/gtcrebywsc.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtcgsbzdxz.html

Py:   if not s:
来源：http://hz.zhaomingkeji.xyz/gtdzgwgrws.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.iojbl.cn/gtutusjfhd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hnxiangtu.top/gtoqonwlnw.html

TS:   if (s === "") {}
来源：http://hz.pycfn.com/gtkoqueljf.html

Java: if (s.isEmpty()) {}
来源：http://hz.yj20258888.top/gtzibvzamb.html

Go:   if s == "" {}
来源：http://hz.nanxuanxn.top/gtqzptdiax.html

Ruby: if s.empty?
来源：http://hz.jqgufenzy.top/gtadhcthfq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xuetiantiany.cn/gtugyrtivb.html

[E21] 超长截断加省略号
来源：http://hz.yangfankeji.com/gtnvnlcxhx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ybcxt.top/gtdrdgadwi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sxryk.cn/gtgdwuhsqa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtcmiexyon.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgfzy.top/gtrzdwspus.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtaqtfbnov.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxinkj.top/gtqkvjyfgh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gttoagzrfs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.havefunace.top/gtodehpcle.html

[E22] 字节长度与字符长度
来源：http://hz.redwolf501.top/gtsklgncvn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.aizwys.cn/gtyvpzsfnb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtfhlzuywa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtvkbziqij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sxryk.cn/gttrardjkf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.smart0.xyz/gtekrxryvj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtjuhwalzo.html

Ruby: s.bytesize;  s.length
来源：http://hz.tanke756.top/gtymcfxhoq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.kuanghao11.cn/gthwjayupd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvlrqormo.html

F. 文件与目录
来源：http://hz.jinyuanbaomall.cn/gtskehabqz.html

================================================================================
来源：http://hz.yongpay.top/gtndswsmaz.html

[F01] 读取整个文件
来源：http://hz.hywenlv.cn/gtatxyflbj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.gogol.net.cn/gthpbgfvec.html

PHP:  file_get_contents("a.txt");
来源：http://hz.smart0.xyz/gtyejkgzia.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ybcxt.top/gtenppgwld.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtewfxefhh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhixingplan.top/gtwnktxskj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.andypj.xyz/gtdtrcatdw.html

Ruby: File.read("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtljnallqu.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.c1oappe.top/gtrfqdxcnu.html

[F02] 逐行读取文件
来源：http://hz.xziqi.cn/gtxhwsnqpm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jianghu66.top/gtqwmrfjhw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.ywan-chungtsiang.top/gtxiijvjbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtutddrltr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtfqswkosx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gtsfsemnhs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.haohaochexian.top/gtiytxgebu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgfzy.top/gtodndddqg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydjk.org.cn/gtgobfxuxb.html

[F03] 写入文件（覆盖）
来源：http://hz.xziqi.cn/gtweepaxyt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yangfankeji.com/gtkclkawxz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtoztoywiy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yonumen.top/gtmvnputei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnxiangtu.top/gtfozwtnqz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.cdnleiting.top/gtxecyixsi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.redwolf501.top/gtvdjatnao.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuetiantiany.cn/gtoepxzprn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cheryme.top/gtakvhtvot.html

[F04] 追加写入文件
来源：http://hz.yuanzhike.top/gtnqnuxvyg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.iojbl.cn/gtlcdrqnfj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shangyingyoupin.top/gtoxruxaid.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9152youxi.cn/gtegeumrsr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sysykeji.top/gtoiwavwyp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtzgjzzgai.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jianghu66.top/gtpscoriqf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtrxnkmsih.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.guannengcc.top/gtpiddtoqj.html

[F05] 判断文件或目录是否存在
来源：http://hz.shangyingyoupin.top/gtecdtekao.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hywenlv.cn/gtocogfprq.html

PHP:  file_exists("a.txt");
来源：http://hz.ehwqpu.com/gtqyirsikc.html

JS:   fs.existsSync("a.txt")
来源：http://hz.chenlongwang.top/gtalziobhi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtjzblkqab.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.tian-w.cn/gtyagboraa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.birdmap.top/gtylkberec.html

Ruby: File.exist?("a.txt")
来源：http://hz.bjfxy.top/gtsiahxjbv.html

C#:   File.Exists("a.txt")
来源：http://hz.tianlin.xyz/gtncbcmrhv.html

[F06] 删除文件
来源：http://hz.wangdashe.top/gtxzcovqci.html

Py:   os.remove("a.txt")
来源：http://hz.nanxinkj.top/gtffvidlfr.html

PHP:  unlink("a.txt");
来源：http://hz.jinghuilouyu.cn/gtnztoloyr.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.vqdsnc.cn/gtnjvybske.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtkljnuxkj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtxqvpfxox.html

Go:   os.Remove("a.txt")
来源：http://hz.yj202588.top/gtxsahggug.html


<!-- 参考信息 -->