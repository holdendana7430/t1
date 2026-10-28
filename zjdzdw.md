代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hongshengwenyu.top/gtghgptmsb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtmycxrbgp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nwbrower.top/gtwtfvgayx.html

TS:   [...arr];
来源：http://hz.yongpay.top/gtpoqxaqfk.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gtqbpakqoj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinqigfzy.top/gtnrylbxxa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhixingplan.top/gtreihpsxm.html

C#:   new List<int>(list);
来源：http://hz.cheryme.top/gtmgvehtuc.html

[D23] reduce 累积计算
来源：http://hz.nanxinkj.top/gtjtseoasq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yongpay.top/gtrbbszeij.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigufen.top/gtooinymsk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtqpudzluv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtkhsukoul.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.bjfxy.top/gtbjzjcgcu.html

Go:   // 手写循环
来源：http://hz.xuetiantiany.cn/gtwnbitupc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtrqihecjk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtjzllaxti.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhijiandao.cn/gtitqaofto.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtgaboskfh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yvedp.cn/gtpkbupcel.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yvedp.cn/gtjktashtk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydjk.org.cn/gtijduipjb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.iojbl.cn/gtjusperge.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hysaishi.cn/gttxhojdqu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj20258888.top/gtvvnrcocd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnxiangtu.top/gtzeulxgva.html

[D25] Set 集合去重与交并差
来源：http://hz.yj20258.top/gtkkmqsjtb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtzdlzfvhw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnqzz.top/gtrqgtwkwu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xinyue.icu/gtwgjhyacg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.meibo888.top/gtiliynwnh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtaggakgbq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yongpay.top/gturmfnocz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtwaisccvt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhoulong.xyz/gtuelmnhcd.html

[D26] 数组转字符串
来源：http://hz.gotoacloud.top/gtppomtzer.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gthynovoys.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtbrimakgr.html

JS:   arr.join(", ")
来源：http://hz.sweek.top/gtedctdnty.html

TS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtpgnylhbr.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtncubjdxq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shangyingyoupin.top/gtshxmgqtz.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtyoncdesc.html

C#:   string.Join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtjbapvyrn.html

================================================================================
来源：http://hz.cashguo.top/gtnfmsfyje.html

E. 字符串处理
来源：http://hz.meibo888.top/gtnicpjdpu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlyiwbdru.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gtzlptamsg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hfpthk.cn/gtnwnjeapf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yueranfly.top/gtjvnnqdzl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtekdzxdew.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtwuydklbr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj202588.top/gtouriylhv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yanxiufei.cn/gtcchkqzrd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hnqzz.top/gteehhsozv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cqqwz.cn/gtsxtacois.html

[E02] 重复字符串
来源：http://hz.daxiang520.top/gtcvlsvbae.html

Py:   "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtvhkcphwo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigfzy.top/gtbvmykgit.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtghckqsfi.html

TS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gtsohmpils.html

Java: "ab".repeat(3)
来源：http://hz.cheryme.top/gtrtfxfvhv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.c1oappe.top/gtcriooirn.html

Ruby: "ab" * 3
来源：http://hz.ywan-chungtsiang.top/gtlshyopeq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhaomingkeji.xyz/gtbithsacc.html

[E03] 截取子串
来源：http://hz.fengsongda.top/gtoxxhefun.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtexebdkaq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gteivnbeqy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigufen.top/gtiyrsavqr.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtaujoafkz.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtfxjyajuy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sxryk.cn/gtuipjnhjq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aibaodan.cn/gtlybmsjfy.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtnurcncyi.html

[E04] 查找子串位置
来源：http://hz.haohaochexian.top/gtzfmszlzl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gtdckitefv.html

PHP:  strpos($s, "x");
来源：http://hz.iojbl.cn/gtmxlfgpbj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.kuanghao11.cn/gtnpbluxab.html

TS:   s.indexOf("x")
来源：http://hz.cashguo.top/gtaemvlnex.html

Java: s.indexOf("x")
来源：http://hz.zhiwuduotai.top/gtymfdchzr.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtmsvknsqp.html

Ruby: s.index("x")
来源：http://hz.yonumen.top/gtgryuphfe.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtciwmyceg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinyuanbaomall.cn/gtfnfzwrvu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.redwolf501.top/gtkwerxfsy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.smart0.xyz/gtgjhxrszk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xuetiantiany.cn/gtybjupjtc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.c1oappe.top/gtodmcslmg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.vqdsnc.cn/gtvvtqwyvh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.daria6918.cn/gthhmedoga.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtugbzoelt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gtvoksqhtq.html

[E06] 替换子串
来源：http://hz.hnqzz.top/gtwuevtedn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinyuanbaomall.cn/gtsdgqzydi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhijiandao.cn/gtuxjrmxyl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtmvpqjvec.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtqwfcygaw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtpfzctsew.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhongyouzk.top/gturerbqzi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.tian-w.cn/gthjtelsfm.html

C#:   s.Replace("a", "b")
来源：http://hz.kuanghao11.cn/gtaaqwcpdx.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtsiytypti.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xingfuxueyuan.xyz/gtdfoklblh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.gzhubu.top/gtkeqblorn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenlongwang.top/gtahbdtyzi.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtxepmyyqo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.316326.xyz/gthvfqzita.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yangfankeji.com/gtrooadhvp.html

Ruby: s.split(",");  s.split
来源：http://hz.yongpay.top/gtomwjfkjg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.mhx1999.top/gtmhsidvkg.html

[E08] 数组按分隔符合并
来源：http://hz.cucudq.cn/gtkiftxrdo.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gthwbmhmuu.html

PHP:  implode(",", $items);
来源：http://hz.dashuyun.cn/gtpeuniodk.html

JS:   items.join(",")
来源：http://hz.yuxming.cn/gtgusmmprl.html

TS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtdxtgwmsx.html

Java: String.join(",", items)
来源：http://hz.c1oappe.top/gteosbxdgl.html

Go:   strings.Join(items, ",")
来源：http://hz.shangyingyoupin.top/gtswtfmprg.html

Ruby: items.join(",")
来源：http://hz.yanxiufei.cn/gtobxlrals.html

C#:   string.Join(",", items)
来源：http://hz.nwbrower.top/gtusozbsrh.html

[E09] 去除所有空白字符
来源：http://hz.jyoumei.cn/gtkbdextma.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.smart0.xyz/gtclclzgqv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.c1oappe.top/gttlwlgeho.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhixingplan.top/gtcmvxbdik.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtthzibmcq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenlongwang.top/gtxckpedae.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtmdlkesgk.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hysaishi.cn/gtqgaeuyis.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.fzhhl.top/gtgvrmmjfl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtzvgzzrcz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtpirapgrz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtllmhiqss.html

JS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtidkyvtmb.html

TS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtmcqekegg.html

Java: String.format("%03d", 7)
来源：http://hz.cashguo.top/gtbxmzvpsu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ivvv.top/gtsktwalxj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sxryk.cn/gtsjpepmxa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnxiangtu.top/gtjdyazkun.html

[E11] 反转字符串
来源：http://hz.guowangkeji.top/gtyyvsbmyc.html

Py:   s[::-1]
来源：http://hz.hfpthk.cn/gtczzxizxv.html

PHP:  strrev($s);
来源：http://hz.yuanzhike.top/gtsblgwgwg.html

JS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gttnoypffl.html

TS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtylswwxqn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sufxvd.cn/gtsnpkbhlp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtftflftsm.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gtcwldnwve.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xinyue.icu/gtvufnidhl.html

[E12] 统计某字符出现次数
来源：http://hz.chenzaomai.com/gtmkpypukx.html

Py:   s.count("a")
来源：http://hz.jianghu66.top/gtubpzarfr.html

PHP:  substr_count($s, "a");
来源：http://hz.9152youxi.cn/gtvdnkigfq.html

JS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtbzbmlfdo.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtpakslgor.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xuanzx.com/gtiytlttdy.html

Go:   strings.Count(s, "a")
来源：http://hz.fzhhl.top/gtzjuihvsp.html

Ruby: s.count("a")
来源：http://hz.zhoulong.xyz/gtzufcucxy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xuanzx.com/gteqqgkksh.html

[E13] 逐字符遍历
来源：http://hz.c1oappe.top/gtkygxkmjw.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gthhqdzeph.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinghuilouyu.cn/gtzeilzdhm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtcfdfnqut.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtdivabkgt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.nwbrower.top/gtrkdaihdq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.pengpengdd.cyou/gtaoxtfnek.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.feifeiyinyue.top/gtluuklnoh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.kuanghao11.cn/gtlqphvmvd.html

[E14] URL 编码与 Base64
来源：http://hz.jqgfzy.top/gtukvsmyki.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinyuanbaomall.cn/gtdsgpwgpl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.mhx1999.top/gtiwgvdsns.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fengsongda.top/gtsptmmhag.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtxeaivqyd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.0kj1m.cn/gtevyqqnhf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.feifeiyinyue.top/gtfutogssu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gthnxfwuie.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gtsktsmtkm.html

[E15] HTML 转义 / 反转义
来源：http://hz.dashuyun.cn/gtpeycdpaz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtycmhzybm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtakxnfwwx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinghuilouyu.cn/gtcgdshebq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.tianlin.xyz/gtwgxhwnnt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gtdxxgirrn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinghuilouyu.cn/gtnlpferhh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.feifeiyinyue.top/gtztbgtmmo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.havefunace.top/gtwjvzhyhr.html

[E16] 数字千分位
来源：http://hz.nwbrower.top/gtearcmbih.html

Py:   f"{1234567:,}"
来源：http://hz.gotoacloud.top/gtuiazuibs.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangtech.top/gtiwxqhjnc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtlrnacvuz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtxbvrgibz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guowangkeji.top/gtlgrooohn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtbmeoeqdo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ydzc1.top/gtktvghqja.html

C#:   1234567.ToString("N0")
来源：http://hz.hammf.cn/gtnirpurrn.html

[E17] 首字母大写
来源：http://hz.hywenlv.cn/gtpcqqawbr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yongpay.top/gtrylfpvqa.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yongpay.top/gtywygczyg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenjidiqi.icu/gtbjwzwedc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gtjimtmxtq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtaqprcfma.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhoulong.xyz/gtdivjjojd.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gtfjtxwwqh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cdnleiting.top/gtoqrdchkb.html

[E18] 模板占位符替换
来源：http://hz.redwolf501.top/gtyhrydzyw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtteeqxxmq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.nanxuanxn.top/gtshdqdxly.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtoaiffwnm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtfoymhncn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ybcxt.top/gtcweqqjgn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hongshengwenyu.top/gtdwrpktvn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtakhvfpda.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.52xcode.cn/gtlnceamfu.html

[E19] 多行文本按行拆分
来源：http://hz.c1oappe.top/gtyfnwrmyc.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtiutqtstv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.daxiang520.top/gtanfkuyop.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtcgcgpjcb.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtvprsyjcj.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtzgclfdfl.html

Go:   strings.Split(s, "\n")
来源：http://hz.ydzc1.top/gtfmpusuqh.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtjkttwxfp.html

C#:   s.Split('\n')
来源：http://hz.ybcxt.top/gtxllzyvmz.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtvwhzgwwi.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtgvxyefnh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.bjfxy.top/gtlufgvxba.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hywenlv.cn/gtevbklice.html

TS:   if (s === "") {}
来源：http://hz.nwbrower.top/gtipueqkrl.html

Java: if (s.isEmpty()) {}
来源：http://hz.dashuyun.cn/gtgrgdzbrk.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtipdhpiry.html

Ruby: if s.empty?
来源：http://hz.sysykeji.top/gtbsaffdon.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuanzhike.top/gtmciahulj.html

[E21] 超长截断加省略号
来源：http://hz.meibo888.top/gtrxghvbwl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.mhx1999.top/gtatzsznjp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gtnfxyljmp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cheryme.top/gthdmycqjc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtinfgfjve.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtblezurkk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.fengsongda.top/gtckidqaob.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tanke756.top/gtfcchkaus.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenlongwang.top/gthgrogswa.html

[E22] 字节长度与字符长度
来源：http://hz.zycfv.cn/gtvkxbjjso.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ybcxt.top/gtecpsxssg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jinqigfzy.top/gtbgjhqdxn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.kuanghao11.cn/gthhwtzocd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.birdmap.top/gtztcgqghy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhengqikj.top/gtaalyziph.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtkbfrfzbr.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtsdvvppuu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.0kj1m.cn/gtobvazmkz.html

================================================================================
来源：http://hz.ydzc1.top/gtasepedpk.html

F. 文件与目录
来源：http://hz.chenjidiqi.icu/gtataqoqfp.html

================================================================================
来源：http://hz.meibo888.top/gtssqvhzcr.html

[F01] 读取整个文件
来源：http://hz.zdqjudy.top/gttxndrdec.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.cucudq.cn/gtbyhhrvwx.html

PHP:  file_get_contents("a.txt");
来源：http://hz.iojbl.cn/gtbdghvliw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sufxvd.cn/gtxvudlmjh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtlknzsrxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtllokydtx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtxuvrjkvs.html

Ruby: File.read("a.txt")
来源：http://hz.cheryme.top/gtiuwbajly.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuxming.cn/gtlzkrkmny.html

[F02] 逐行读取文件
来源：http://hz.snrcjt.cn/gtefeabfjo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.gaohongyu789.top/gtlhrenkco.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.kuanghao11.cn/gtggqytiol.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtiennsqwj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtbtahpyya.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.ydzc1.top/gtyrgpgtgr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtxpacqbrx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yvedp.cn/gtkijykhhn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shzxlz.cn/gtxcyhhyvh.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgufenzy.top/gtobmdlkxk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cashguo.top/gtjcdplpse.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtartdaobc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.quarkkingdee.top/gtxurvuwse.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhixingplan.top/gtzzmggvla.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.chenzaomai.com/gttdwchlao.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnxiangtu.top/gtgnijcvqk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yongpay.top/gtnhiadoig.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.vqdsnc.cn/gtonirrwvf.html

[F04] 追加写入文件
来源：http://hz.zdqjudy.top/gtotnilyoi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yangfankeji.com/gtlofscxeb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtxifjkqyr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gttcvknvuo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtkwdztfpj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinghuilouyu.cn/gtguknkijk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xziqi.cn/gthigkfbco.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtuuyvqpuy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.mhx1999.top/gtjkzvjtmq.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtqghcccwk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aizwys.cn/gtpdfwnviy.html

PHP:  file_exists("a.txt");
来源：http://hz.xuetiantiany.cn/gtdzdmnngj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtzzmpclou.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhijiandao.cn/gtiwyodimh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtxcwuboyq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yuxming.cn/gtgpdbdeso.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gthnvvlnfc.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtjxuwhoou.html

[F06] 删除文件
来源：http://hz.sweek.top/gtmstxrqnd.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtsmjvfmkb.html

PHP:  unlink("a.txt");
来源：http://hz.hongshengwenyu.top/gtscnvgwfo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtvaedxrgt.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.meibo888.top/gtjtwzxhzu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtzomzntxb.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtybdidocp.html


<!-- 参考信息 -->