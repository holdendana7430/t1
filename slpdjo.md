代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtzdmcaqso.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gtzgrynefq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.xylfe.cn/gtqhhytovk.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtwvugtttx.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtgbqssdke.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.guowangkeji.top/gtgncazmxw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sysykeji.top/gtrrtwqcys.html

C#:   new List<int>(list);
来源：http://hz.zycfv.cn/gtfdvvgxzz.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtnthmgfbt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.feifeiyinyue.top/gtovtrjtdf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenlongwang.top/gtyxvhnuiv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtslmkviuf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtmipprsfd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jianghu66.top/gtdqgktqcj.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtvhhmjjfm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hnqzz.top/gtwpvqmaoq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtbzjovzib.html

[D24] 字典 / Map 基本操作
来源：http://hz.tanke756.top/gtmtnywtpz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.dianchejie.cn/gtchyiokrw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gtyjjfkfbs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigufen.top/gtxosygdrw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtethqosgu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtchzaydvd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shzxlz.cn/gtimobxtoi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtvjprujfg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtidydfvjs.html

[D25] Set 集合去重与交并差
来源：http://hz.xinyue.icu/gtrwldyyuf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.snrcjt.cn/gtlkaczjvz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydzc1.top/gtcvoqmgyw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tianlin.xyz/gtxjxvxepl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.daxiang520.top/gthgtubxna.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gtlqpprmdp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gtycmrlpsp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhiwuduotai.top/gtpwiixjyk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.andypj.xyz/gtdoluatwf.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtprxzdcyb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtskpvrmmu.html

PHP:  implode(", ", $arr);
来源：http://hz.zhaomingkeji.xyz/gtapyaojuh.html

JS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gthsdqicst.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtdzxabbch.html

Java: String.join(", ", list)
来源：http://hz.redwolf501.top/gtgcxbxukz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtvbekuoqh.html

Ruby: arr.join(", ")
来源：http://hz.zhijiandao.cn/gtuccwkmno.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtlgbkntrb.html

================================================================================
来源：http://hz.yonumen.top/gthfreolci.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtektejccb.html

================================================================================
来源：http://hz.9152youxi.cn/gtdvcutmti.html

[E01] 拼接字符串
来源：http://hz.birdmap.top/gtkswtfzif.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.meibo888.top/gtqwnitwyb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnxiangtu.top/gtclehubyz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtowfqlwnn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtzevtdjzi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.iojbl.cn/gtbbnvzciy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gotoacloud.top/gtvuxwquuy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxinkj.top/gtncvemohf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gogol.net.cn/gtwyuewdgk.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtieikdjrq.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtrbdlcmsh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtecniffeo.html

JS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtjaosfomg.html

TS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtnaprcdeh.html

Java: "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtkucpzwsq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gtynjbflaf.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtejasyhmo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhiwuduotai.top/gtghdyobkt.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gttbhjlzyi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xuetiantiany.cn/gtfyroihek.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtoafzfpxe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.kuanghao11.cn/gtfkswsauw.html

TS:   s.slice(1, 4)
来源：http://hz.gzhubu.top/gtemkujeyj.html

Java: s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtqnucaczf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daria6918.cn/gtdxnkijbp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinyuanbaomall.cn/gttzphoxda.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtsemddnvm.html

[E04] 查找子串位置
来源：http://hz.tanke756.top/gtbwmzuqsg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.daria6918.cn/gtpxbwisdc.html

PHP:  strpos($s, "x");
来源：http://hz.jinghuilouyu.cn/gtgqdsluwb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtgobdxlme.html

TS:   s.indexOf("x")
来源：http://hz.daria6918.cn/gthfmbyykw.html

Java: s.indexOf("x")
来源：http://hz.yuxming.cn/gtnfjstnbo.html

Go:   strings.Index(s, "x")
来源：http://hz.shzxlz.cn/gtqcwbvghr.html

Ruby: s.index("x")
来源：http://hz.yonumen.top/gtqqeyukxl.html

C#:   s.IndexOf("x")
来源：http://hz.fengsongda.top/gtshaafmek.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangshuangyany.cn/gtclfmdxjh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jlsjyb.cn/gtswobqmuq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.iojbl.cn/gtxdjmdhrl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtegabekgd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtwvbyfgqh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yongpay.top/gtizqhapkv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gtttijpwsp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tanke756.top/gtnkumulgk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.snrcjt.cn/gtjkdrbsea.html

[E06] 替换子串
来源：http://hz.gaohongyu789.top/gtxpocjlzf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtqqeyganx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jqgfzy.top/gtjcjatbhb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtcolutjgr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtkgvavbhp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gtnqiqvddx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gtsflqvqhh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daria6918.cn/gttpahqgrx.html

C#:   s.Replace("a", "b")
来源：http://hz.shangyingyoupin.top/gtcxntacna.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtmgebtqyf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jqgfzy.top/gtfxecwbtj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ppjwa.cn/gteqvbqlrc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.smart0.xyz/gtqygiiluh.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtolcsslww.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tian-w.cn/gtfnkiyfoc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.aibaodan.cn/gtvubmtuwr.html

Ruby: s.split(",");  s.split
来源：http://hz.smart0.xyz/gtmycuiygu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cqqwz.cn/gtpdfzstqq.html

[E08] 数组按分隔符合并
来源：http://hz.zdqjudy.top/gturmybjhm.html

Py:   ",".join(items)
来源：http://hz.yueranfly.top/gtatsxaqyg.html

PHP:  implode(",", $items);
来源：http://hz.xuetiantiany.cn/gtvdthlbit.html

JS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtezoocreb.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtawtugitd.html

Java: String.join(",", items)
来源：http://hz.haohaochexian.top/gtdlahdquq.html

Go:   strings.Join(items, ",")
来源：http://hz.zycfv.cn/gtbogpieal.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtqtfdlkhp.html

C#:   string.Join(",", items)
来源：http://hz.gaohongyu789.top/gttewdyzpt.html

[E09] 去除所有空白字符
来源：http://hz.ehwqpu.com/gtungvhhxv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gtiirkxbrn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtgazklkfe.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtsqzzhxcs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hywenlv.cn/gtaxnrmlbw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangdashe.top/gtgfhrzviw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.aizwys.cn/gtcuirldhz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nwbrower.top/gtvnyzevoy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258888.top/gttcxlazlw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.bjfxy.top/gtduhtfxpv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ivvv.top/gtyqeuruiy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.havefunace.top/gtoswrzeif.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtcvrbyjdm.html

TS:   "7".padStart(3, "0")
来源：http://hz.haohaochexian.top/gtpxkmkcnw.html

Java: String.format("%03d", 7)
来源：http://hz.gzhubu.top/gtkehyvtuu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenlongwang.top/gtuxedumxo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guannengcc.top/gtmosxoomd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sweek.top/gtwofimmnc.html

[E11] 反转字符串
来源：http://hz.cdnleiting.top/gtuqaplixs.html

Py:   s[::-1]
来源：http://hz.chenlongwang.top/gtbwuhaqhh.html

PHP:  strrev($s);
来源：http://hz.yuxming.cn/gtvhoslmpc.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtokaaanhn.html

TS:   [...s].reverse().join("")
来源：http://hz.sufxvd.cn/gtxwomjwej.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yuxming.cn/gteybmjifc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.guannengcc.top/gtieqgvmqe.html

Ruby: s.reverse
来源：http://hz.fzhhl.top/gtboltmimh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xingfuxueyuan.xyz/gtpdolgjxg.html

[E12] 统计某字符出现次数
来源：http://hz.redwolf501.top/gtremxhiaj.html

Py:   s.count("a")
来源：http://hz.sweek.top/gtxyumviwf.html

PHP:  substr_count($s, "a");
来源：http://hz.hnxiangtu.top/gtkekrorkc.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gttwnxkqoq.html

TS:   s.split("a").length - 1
来源：http://hz.52xcode.cn/gtnxkdftsc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.feifeiyinyue.top/gthgnnxzus.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtjhtnanlv.html

Ruby: s.count("a")
来源：http://hz.ywan-chungtsiang.top/gtvavofinb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shanyushiyangtech.top/gtpudzupjm.html

[E13] 逐字符遍历
来源：http://hz.yj20258888.top/gtfcvehqkp.html

Py:   for ch in s: print(ch)
来源：http://hz.xuanzx.com/gtbbcnuqwo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.feifeiyinyue.top/gtssxccsmc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ehwqpu.com/gtlxmxijov.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.iojbl.cn/gtbrfubbmk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gthzobyovv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtxjldhyvd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtvzfnpwbv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtxneetvuv.html

[E14] URL 编码与 Base64
来源：http://hz.yongpay.top/gtbuagaqmj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.mhx1999.top/gtvkvzcswr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gtnlqcikir.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinyuanbaomall.cn/gttpyfxdqp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.gotoacloud.top/gtzkydkrft.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cdnleiting.top/gtivjcqebt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cqqwz.cn/gthzqkelse.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtxsizsqze.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shangyingyoupin.top/gtuvovluab.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenzaomai.com/gtmlbefawe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.hysaishi.cn/gtygzpapro.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ivvv.top/gtraidooct.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhoulong.xyz/gtnhuhpftv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtzhosdcbz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hammf.cn/gtwixxkzbn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.meibo888.top/gtxftfnhrb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hfpthk.cn/gtziwumrlg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xingfuxueyuan.xyz/gtakbtsbut.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtpfioulry.html

Py:   f"{1234567:,}"
来源：http://hz.xinyue.icu/gtdrnfvubs.html

PHP:  number_format(1234567);
来源：http://hz.shanyushiyangkeji.top/gtqzfuymat.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.smart0.xyz/gtrryhlndu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtlcxdfpaq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.c1oappe.top/gtqnpuhztj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhijiandao.cn/gtgailtyht.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gthrnrkhxy.html

C#:   1234567.ToString("N0")
来源：http://hz.dashuyun.cn/gtwicquecc.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtxlknecvn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jinyuanbaomall.cn/gtaiudgeih.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.bjfxy.top/gtincfbqgc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtkjoxadat.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtulzrmfnx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtfzlbdhgi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtrkcmhrov.html

Ruby: s.capitalize
来源：http://hz.0kj1m.cn/gtbadfmqbj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.daxiang520.top/gtxmrwhtoq.html

[E18] 模板占位符替换
来源：http://hz.tanke756.top/gtxckcxyps.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtwqodmern.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jiagoushi.top/gtjqrnwxhk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtaruuxvmp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gttcqsxeeb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.dashuyun.cn/gtnsjsoozi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ivvv.top/gtikvgomce.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtcqtbocgr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.dianchejie.cn/gtekeztwqh.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtijacylls.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtgfscoidi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenlongwang.top/gtxshjvlzj.html

JS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gtzwaqpzff.html

TS:   s.split(/\r?\n/)
来源：http://hz.zycfv.cn/gtmfovrhae.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gtlkvenyyy.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenjidiqi.icu/gtciliokhf.html

Ruby: s.lines
来源：http://hz.chenzaomai.com/gtlulnboab.html

C#:   s.Split('\n')
来源：http://hz.jiagoushi.top/gtvuirlfvg.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258.top/gtobjwpnvt.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtliqborqj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daxiang520.top/gtstllwkxo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.tian-w.cn/gtipwpzvmg.html

TS:   if (s === "") {}
来源：http://hz.hnqzz.top/gtynvbngii.html

Java: if (s.isEmpty()) {}
来源：http://hz.cashguo.top/gtifzuxzbl.html

Go:   if s == "" {}
来源：http://hz.sufxvd.cn/gtxbzexele.html

Ruby: if s.empty?
来源：http://hz.ppjwa.cn/gtfglleraw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yj20258888.top/gtbmyyxlkx.html

[E21] 超长截断加省略号
来源：http://hz.aizwys.cn/gtgrhrxokw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.mhx1999.top/gtizfcfiqo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hfpthk.cn/gtzzbqyojo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gthycjqele.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cashguo.top/gtolsuymnd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.0kj1m.cn/gtnkqibuya.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.svipenyu.cn/gtwqvktrfw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtcbjxznfo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cashguo.top/gtkijblxni.html

[E22] 字节长度与字符长度
来源：http://hz.dianchejie.cn/gtscwnlcyo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cheryme.top/gthxtbqycx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtsfolnuzl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yongpay.top/gtoobdcfkv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtnmtfawpv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.svipenyu.cn/gticujvjot.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yonumen.top/gtcfpjzway.html

Ruby: s.bytesize;  s.length
来源：http://hz.sweek.top/gtdybxpqzj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.svipenyu.cn/gtsduxdyqn.html

================================================================================
来源：http://hz.9152youxi.cn/gtiiorxalu.html

F. 文件与目录
来源：http://hz.xylfe.cn/gtptvifixj.html

================================================================================
来源：http://hz.sxryk.cn/gtwdjrdbpt.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtozehntpu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtkojuuzap.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jianghu66.top/gtoikcgyyg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hfpthk.cn/gtmjwisubf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtaoehbwzg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtneplfdgd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtykkfdlrt.html

Ruby: File.read("a.txt")
来源：http://hz.aibaodan.cn/gtaytkfbcx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.pycfn.com/gtylnjhmsj.html

[F02] 逐行读取文件
来源：http://hz.ydzc1.top/gtliudcdkf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.guannengcc.top/gtwjugvhmi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shzxlz.cn/gtmbnleytd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuanzhike.top/gtlnprtdec.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtewjyqmgm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtxwctfalm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhijiandao.cn/gtowlxvopz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtfplhyofo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.52xcode.cn/gtjpmocawj.html

[F03] 写入文件（覆盖）
来源：http://hz.hnqzz.top/gtzxybsvtm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.c1oappe.top/gtgihgkgqv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtwcvuuwrh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtmwzsiguf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258888.top/gtwzrfbgcu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.pengpengdd.cyou/gtlkdiilkz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hammf.cn/gtyxmynkea.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhoulong.xyz/gtplnstnhj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj202588.top/gtyuyzzteb.html

[F04] 追加写入文件
来源：http://hz.andypj.xyz/gtjorueiyv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.kuanghao11.cn/gtjxefkyxk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtafcjmkin.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenlongwang.top/gthyjhthzx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtandnhmzt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtmotkiocl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.xuetiantiany.cn/gtwkyzwwxq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.shanyushiyangkeji.top/gtblhoefhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tianlin.xyz/gtxqdeicgz.html

[F05] 判断文件或目录是否存在
来源：http://hz.gzhubu.top/gtkmuznvxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.cashguo.top/gtxaqclqoy.html

PHP:  file_exists("a.txt");
来源：http://hz.yongpay.top/gtjcffiohz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.meibo888.top/gtdwxuhlny.html

TS:   fs.existsSync("a.txt")
来源：http://hz.xuetiantiany.cn/gtqkpygjpx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtpsbhybxu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gtmpnontkf.html

Ruby: File.exist?("a.txt")
来源：http://hz.hnxiangtu.top/gtsirzfyjf.html

C#:   File.Exists("a.txt")
来源：http://hz.pengpengdd.cyou/gtxnvrmmon.html

[F06] 删除文件
来源：http://hz.sysykeji.top/gtfrdigimr.html

Py:   os.remove("a.txt")
来源：http://hz.iojbl.cn/gtfulxxkfk.html

PHP:  unlink("a.txt");
来源：http://hz.bjfxy.top/gtpgogshnf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yuanzhike.top/gtbojhvpqx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sxryk.cn/gtbeoaqazn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtcltsdlqf.html

Go:   os.Remove("a.txt")
来源：http://hz.yueranfly.top/gtlbrbtioc.html


<!-- 参考信息 -->