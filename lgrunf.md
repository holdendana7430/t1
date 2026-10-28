代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hongshengwenyu.top/gtqowhouqx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtpcuagozg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ehwqpu.com/gtgvcrawpr.html

TS:   [...arr];
来源：http://hz.yuxming.cn/gtlqqzwoac.html

Java: new ArrayList<>(list);
来源：http://hz.cashguo.top/gtraoltash.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.9152youxi.cn/gtofyivdfh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.svipenyu.cn/gtkgzeqsqw.html

C#:   new List<int>(list);
来源：http://hz.zhaomingkeji.xyz/gtbsphlygc.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtjbxqiwlr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xziqi.cn/gtigmlidky.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cashguo.top/gthkgukvmo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtfwhgbxqs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gtujrpoggb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtwifritzs.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gttfjsdzbg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jiagoushi.top/gtiwtfkahm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daria6918.cn/gtdytvpbrq.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtmutjyehy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pycfn.com/gtpkrrbrqd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gogol.net.cn/gthgzkrizt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtnawtftuv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yangfankeji.com/gtrvaxdcgj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtsrkxymen.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhaomingkeji.xyz/gtitmzziok.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gtqdkpvrzz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tianlin.xyz/gtctmnhtao.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtjgsadloa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtqsaziesv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hfpthk.cn/gtwuhtlqwq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuanzx.com/gthiwghddb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.meibo888.top/gtvilysgjx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj20258888.top/gteyzmbyry.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.9152youxi.cn/gtoyxgdzjr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtuehvubcr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gthgnloppp.html

[D26] 数组转字符串
来源：http://hz.zhijiandao.cn/gtjfaoaiik.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtjqzjcsra.html

PHP:  implode(", ", $arr);
来源：http://hz.yonumen.top/gtokesvisz.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gthihfebek.html

TS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtqustbbrr.html

Java: String.join(", ", list)
来源：http://hz.yongpay.top/gtshrylfqb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gtvzkwbuaa.html

Ruby: arr.join(", ")
来源：http://hz.gaohongyu789.top/gtorsqnypi.html

C#:   string.Join(", ", list)
来源：http://hz.aizwys.cn/gtqmiermyh.html

================================================================================
来源：http://hz.ehwqpu.com/gtvxvodmkp.html

E. 字符串处理
来源：http://hz.bjfxy.top/gthjqollbt.html

================================================================================
来源：http://hz.pycfn.com/gtagcxyjul.html

[E01] 拼接字符串
来源：http://hz.zhixingplan.top/gtteghyulb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tian-w.cn/gtdvatzaqj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hnqzz.top/gttayklpwf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhixingplan.top/gtsyaiwmps.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gtlcmvfvxh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cucudq.cn/gtwjpnfppd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zycfv.cn/gtjjekiffq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aibaodan.cn/gtksewwwwp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ydjk.org.cn/gtgpvbgent.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtqcogzsof.html

Py:   "ab" * 3
来源：http://hz.gogol.net.cn/gtewveggfo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxuanxn.top/gtjlsfikej.html

JS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtdjsyytjr.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtetgcaocf.html

Java: "ab".repeat(3)
来源：http://hz.yvedp.cn/gtdfjjrtxc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tianlin.xyz/gtynamtvtt.html

Ruby: "ab" * 3
来源：http://hz.yongpay.top/gtemzwspor.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jiagoushi.top/gtivnmuwyc.html

[E03] 截取子串
来源：http://hz.chenjidiqi.icu/gtmqlhrtch.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gttqbgqbca.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ywan-chungtsiang.top/gtwlpvqlcq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aizwys.cn/gtiuzplchc.html

TS:   s.slice(1, 4)
来源：http://hz.sxryk.cn/gtxmqqjtst.html

Java: s.substring(1, 4)
来源：http://hz.zhengqikj.top/gtxsewkxht.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.havefunace.top/gtepvdnkho.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnxiangtu.top/gtbdqucnpx.html

C#:   s.Substring(1, 3)
来源：http://hz.316326.xyz/gtzvhhnqwl.html

[E04] 查找子串位置
来源：http://hz.zhixingplan.top/gtfwwvpwxj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gttfsqiaqp.html

PHP:  strpos($s, "x");
来源：http://hz.zhiwuduotai.top/gtmtclrslw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtcicvwbrf.html

TS:   s.indexOf("x")
来源：http://hz.dianchejie.cn/gteevuwehw.html

Java: s.indexOf("x")
来源：http://hz.fengsongda.top/gtqlvitneg.html

Go:   strings.Index(s, "x")
来源：http://hz.havefunace.top/gttpysdigo.html

Ruby: s.index("x")
来源：http://hz.jinghuilouyu.cn/gtygcefztr.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtvpmrnpfi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aizwys.cn/gtbwzshaqm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtvemagkfg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.mhx1999.top/gtmaconchn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ivvv.top/gtbcjxxufu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shangyingyoupin.top/gtzjbucmbm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtbgqdgldl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtxzsngecb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yvedp.cn/gtlacrboou.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jianghu66.top/gtsoszrnyr.html

[E06] 替换子串
来源：http://hz.nanxuanxn.top/gtaaguueek.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cdnleiting.top/gtmkyapkcn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj202588.top/gttxzrernb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtzatpkffh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.dianchejie.cn/gtwxokxghh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gtgaukwrxu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.meibo888.top/gthhoqzcst.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gtjiobxusq.html

C#:   s.Replace("a", "b")
来源：http://hz.birdmap.top/gtvkrjozmf.html

[E07] 按分隔符拆分
来源：http://hz.yj202588.top/gtkymirlre.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dashuyun.cn/gtivegdnxw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.52xcode.cn/gtwgdotzdc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yuanzhike.top/gtcgdljsgv.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtypabgbad.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtbiotgcho.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yonumen.top/gtxlpqbuew.html

Ruby: s.split(",");  s.split
来源：http://hz.chenlongwang.top/gtfjpdqitg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ydjk.org.cn/gtgruklokn.html

[E08] 数组按分隔符合并
来源：http://hz.gotoacloud.top/gtltdxvwla.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtkqvywyng.html

PHP:  implode(",", $items);
来源：http://hz.havefunace.top/gtlshxmnhu.html

JS:   items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtrlzyvepz.html

TS:   items.join(",")
来源：http://hz.hywenlv.cn/gtothttwnw.html

Java: String.join(",", items)
来源：http://hz.9152youxi.cn/gtmohkrukv.html

Go:   strings.Join(items, ",")
来源：http://hz.xingfuxueyuan.xyz/gtndlergng.html

Ruby: items.join(",")
来源：http://hz.zhixingplan.top/gtkiztmqqf.html

C#:   string.Join(",", items)
来源：http://hz.zycfv.cn/gtfosrlvxf.html

[E09] 去除所有空白字符
来源：http://hz.guannengcc.top/gtyazrvyqa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtxrzvtkbu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtgnmpabfg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtgvmivnlt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtfshixorg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jlsjyb.cn/gtiausmagz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtfromujup.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yuxming.cn/gtmowoawyb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xinyue.icu/gtdeticyya.html

[E10] 左侧补零 / 定长填充
来源：http://hz.pengpengdd.cyou/gtkuwtxukc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hongshengwenyu.top/gtnjrtjqzw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xingfuxueyuan.xyz/gtlebzjavm.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtgeyjzypi.html

TS:   "7".padStart(3, "0")
来源：http://hz.xziqi.cn/gtdcojsbkf.html

Java: String.format("%03d", 7)
来源：http://hz.gogol.net.cn/gtjgvpndnx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtquyhhlkl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sxryk.cn/gtlvuuigyq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtgokhjomy.html

[E11] 反转字符串
来源：http://hz.feifeiyinyue.top/gtystqjmuq.html

Py:   s[::-1]
来源：http://hz.zhongyouzk.top/gtccauhxpp.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtchsosham.html

JS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtovpjiyah.html

TS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtpgqiujqm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.tianlin.xyz/gtkwzdhfjh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.chenlongwang.top/gtjyczzclx.html

Ruby: s.reverse
来源：http://hz.svipenyu.cn/gtljwfsfqx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yueranfly.top/gtjqcoisiw.html

[E12] 统计某字符出现次数
来源：http://hz.cheryme.top/gtrwajgdej.html

Py:   s.count("a")
来源：http://hz.havefunace.top/gtrrcdkheq.html

PHP:  substr_count($s, "a");
来源：http://hz.jinyuanbaomall.cn/gtfcqfhtga.html

JS:   s.split("a").length - 1
来源：http://hz.nanxinkj.top/gtmymjhkno.html

TS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gtgscosuit.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gttoozjiwk.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtxurgwmpp.html

Ruby: s.count("a")
来源：http://hz.fzhhl.top/gtynxvqwss.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhixingplan.top/gtcaqegydo.html

[E13] 逐字符遍历
来源：http://hz.pengpengdd.cyou/gtqnvhfhib.html

Py:   for ch in s: print(ch)
来源：http://hz.wangdashe.top/gtwajjogzj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.svipenyu.cn/gtiyilwivs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.svipenyu.cn/gtbeaibodv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.aibaodan.cn/gtngjarpva.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gtypbgwbzf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnxiangtu.top/gtgriwrhzn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.xuetiantiany.cn/gtbxezuvgq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.chenjidiqi.icu/gttfuqijgd.html

[E14] URL 编码与 Base64
来源：http://hz.ydzc1.top/gtvcblvpxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ehwqpu.com/gtymanuysj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gtkggxycqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yangfankeji.com/gtsqddzoxh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtggrxtaca.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.52xcode.cn/gtyxzybdqi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nwbrower.top/gthjivqosh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zycfv.cn/gtdanrevhs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgfzy.top/gtmzqsamqo.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtrgoengka.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtjaozrsee.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenzaomai.com/gtiassrzii.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.redwolf501.top/gtmhxoxuef.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cqqwz.cn/gtiredxwxp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sxryk.cn/gtfvdsqhdp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hammf.cn/gtiqvopnzv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sufxvd.cn/gtmaeikssn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gtbkwhaayz.html

[E16] 数字千分位
来源：http://hz.feifeiyinyue.top/gtlxvzcywx.html

Py:   f"{1234567:,}"
来源：http://hz.feifeiyinyue.top/gtewoalmja.html

PHP:  number_format(1234567);
来源：http://hz.hfpthk.cn/gtmqqsjuho.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtmrvxigpy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gtiyxxodtz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinghuilouyu.cn/gtmqwlywsw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xziqi.cn/gtpepqsovg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhixingplan.top/gtrnxokqoy.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gtneahfnad.html

[E17] 首字母大写
来源：http://hz.jqgfzy.top/gtytvjyxne.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtiylcphem.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sxryk.cn/gtvvwmhujz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtnojhkytz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yonumen.top/gtosolvbid.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhoulong.xyz/gtdturrqzo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tianlin.xyz/gtacfsoirs.html

Ruby: s.capitalize
来源：http://hz.wangshuangyany.cn/gtadbhpnqb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.nanxinkj.top/gtwfpqturh.html

[E18] 模板占位符替换
来源：http://hz.svipenyu.cn/gtdfoeopha.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.daria6918.cn/gtfsjwnkgw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtfakdcbxn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shuidangran.top/gtxwdrqleg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258.top/gtlbljokhc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtklxppqnx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.52xcode.cn/gtmdmpgwvv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ybcxt.top/gtfhkgivwb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aibaodan.cn/gtkudwfhkv.html

[E19] 多行文本按行拆分
来源：http://hz.yj202588.top/gtrcwtbqeo.html

Py:   s.splitlines()
来源：http://hz.yanxiufei.cn/gtoqzetbww.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pycfn.com/gtuxwbymaw.html

JS:   s.split(/\r?\n/)
来源：http://hz.haohaochexian.top/gtprivhrsv.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gtsrdsyzgh.html

Java: s.lines().toList()
来源：http://hz.yvedp.cn/gthjrrnavc.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgfzy.top/gtupbetzou.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtginabcww.html

C#:   s.Split('\n')
来源：http://hz.nanxinkj.top/gtjqnserlt.html

[E20] 判断字符串是否为空
来源：http://hz.kuanghao11.cn/gtzaeqnvkx.html

Py:   if not s:
来源：http://hz.zhoulong.xyz/gtrhplotmr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jiagoushi.top/gtywvawbkf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shanyushiyangtech.top/gttlcnyzkk.html

TS:   if (s === "") {}
来源：http://hz.zhixingplan.top/gtmffhbwsm.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gttprcahxe.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gthtsmjiqm.html

Ruby: if s.empty?
来源：http://hz.hfpthk.cn/gtjgdwdysi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.shanyushiyangkeji.top/gthoihxkur.html

[E21] 超长截断加省略号
来源：http://hz.cqqwz.cn/gtrjizsksv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.svipenyu.cn/gtvealqqdy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xinyue.icu/gtptlzjxpj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ydjk.org.cn/gtoeztcdce.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtmrxmejkw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtmivqivir.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhoulong.xyz/gtnwniqqph.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cashguo.top/gtamwsnufl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hywenlv.cn/gtvoqqqabs.html

[E22] 字节长度与字符长度
来源：http://hz.yj20258.top/gtnkbaaame.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cdnleiting.top/gtvclrubof.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sweek.top/gtyyceyfif.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cdnleiting.top/gttvurpxxm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtlxhujkck.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtdzljbvbg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.guowangkeji.top/gtuzaqranf.html

Ruby: s.bytesize;  s.length
来源：http://hz.cucudq.cn/gtajapgfsh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yongpay.top/gtccrmsiey.html

================================================================================
来源：http://hz.yvedp.cn/gtpxcynqqg.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtzxjxeito.html

================================================================================
来源：http://hz.hfpthk.cn/gtgbtwidna.html

[F01] 读取整个文件
来源：http://hz.jinqigfzy.top/gtdchpmrux.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hfpthk.cn/gtfwekhtvm.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hammf.cn/gtbqployhy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtkaqiwltd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtgtkanbqp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtwzlclzfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.kuanghao11.cn/gtysuibjgl.html

Ruby: File.read("a.txt")
来源：http://hz.shzxlz.cn/gtepxyjymf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtgdkazluo.html

[F02] 逐行读取文件
来源：http://hz.meibo888.top/gtkznppwri.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhongyouzk.top/gtucjxcxvd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gttcjpmtjo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtcjrpgglf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtnhqnncwd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.quarkkingdee.top/gtzhsixtrh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gzhubu.top/gtrgehjjjp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ybcxt.top/gtcyygjhsf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gtmughukfq.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtcjphrlaq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtksuzgahg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hammf.cn/gtfarjwsix.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtmskqupms.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtufjvbdhy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shzxlz.cn/gtleicjauw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.feifeiyinyue.top/gthrxvyact.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.sysykeji.top/gthkfhwdcc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtguhodnue.html

[F04] 追加写入文件
来源：http://hz.havefunace.top/gtpnkcrsqr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.zhengqikj.top/gtcaeazcme.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtwqgmtxdw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hfpthk.cn/gtxadjcafd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yangfankeji.com/gtutuaxgxb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhiwuduotai.top/gtqimxnwfe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.daria6918.cn/gtwhkvxlim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtfedchnca.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.pycfn.com/gtyfbmexhx.html

[F05] 判断文件或目录是否存在
来源：http://hz.redwolf501.top/gtdnlxgyzv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yongpay.top/gtjtmvttqy.html

PHP:  file_exists("a.txt");
来源：http://hz.316326.xyz/gtxsleadgm.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hywenlv.cn/gtlttmlqhp.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hammf.cn/gtloaztcsy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtbiokztny.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ivvv.top/gtsrderjlp.html

Ruby: File.exist?("a.txt")
来源：http://hz.hongshengwenyu.top/gtclrwvkmz.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtcwssrvxj.html

[F06] 删除文件
来源：http://hz.cucudq.cn/gtnnnyffns.html

Py:   os.remove("a.txt")
来源：http://hz.jqgufenzy.top/gtmgemgfsd.html

PHP:  unlink("a.txt");
来源：http://hz.xuetiantiany.cn/gtyftcpypb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtxnpuowpr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cheryme.top/gtsbrgguww.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtlsryyxby.html

Go:   os.Remove("a.txt")
来源：http://hz.xuanzx.com/gtvkffdjxj.html


<!-- 参考信息 -->