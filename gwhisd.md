代发 wailian999

Ruby: arr.tally
来源：http://hz.jinqigfzy.top/gtkflsyxjh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zdqjudy.top/gtmozokgfw.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtfaxpyffr.html

Py:   x in arr
来源：http://hz.meibo888.top/gtwsqaghmx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtnwisbube.html

JS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtdfzrkkdl.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtdzhxqipq.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtztlbgjmt.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtbqqaqjok.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gtbaugtjoi.html

C#:   list.Contains(x)
来源：http://hz.cheryme.top/gtuxfztmdo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhixingplan.top/gtwpxkjejf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.iojbl.cn/gtoiuquyvo.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenlongwang.top/gtlsvweqaz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gtjatlesxj.html

TS:   [...arr];
来源：http://hz.tanke756.top/gtkyeffwlb.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtyivwonxf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jlsjyb.cn/gtrthgavia.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shanyushiyangkeji.top/gttcgdkflj.html

C#:   new List<int>(list);
来源：http://hz.yj202588.top/gtaacwbulh.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gthfcgctyo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.dianchejie.cn/gtiokdthnw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zdqjudy.top/gttxzasaql.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtidrligwk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtulembjuq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.birdmap.top/gtdkpqoriu.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtajyhipaw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenjidiqi.icu/gtbhummshr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xziqi.cn/gtvkqycvpa.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtdntcexvy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtpgknnwby.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gthigjgizo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtexszozri.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtclpogzbd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.wangshuangyany.cn/gtedxwlmkx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgufenzy.top/gtppfkvyrn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ivvv.top/gtyafkolgl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hongshengwenyu.top/gtxhobspjk.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gthfdsntvh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtyycartmu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhiwuduotai.top/gtgeysryto.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangshuangyany.cn/gtmemltsnw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yongpay.top/gteqwypplj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yvedp.cn/gtufsqbcqr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgufenzy.top/gtlfcpwrvv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yvedp.cn/gtyshpqvfe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhixingplan.top/gtbmbgdycd.html

[D26] 数组转字符串
来源：http://hz.aibaodan.cn/gtaqkyvvwk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tanke756.top/gtakscfcmw.html

PHP:  implode(", ", $arr);
来源：http://hz.jinyuanbaomall.cn/gtvusxzrjh.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtuujwluum.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtoqrfdvqm.html

Java: String.join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtfqbmlluy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gtdxrjynif.html

Ruby: arr.join(", ")
来源：http://hz.dashuyun.cn/gtpgcwoapq.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtmtjknuxe.html

================================================================================
来源：http://hz.hfpthk.cn/gtwuawdmez.html

E. 字符串处理
来源：http://hz.hammf.cn/gtkzenikmk.html

================================================================================
来源：http://hz.gogol.net.cn/gtwdvfpgfh.html

[E01] 拼接字符串
来源：http://hz.xuetiantiany.cn/gtoodccpna.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nwbrower.top/gtyfmltleb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtgfhbrsoc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtunvoijwt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtupwbhzdg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.birdmap.top/gtfuvmqqky.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cucudq.cn/gtxigelfsj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtbmsrxaxe.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sxryk.cn/gtsugpdgwh.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gtqknscshq.html

Py:   "ab" * 3
来源：http://hz.daxiang520.top/gtyqpfkjus.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sysykeji.top/gtsoihhbrv.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gthtkcukwr.html

TS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtxlwhtkgt.html

Java: "ab".repeat(3)
来源：http://hz.sxryk.cn/gtwvzhhnat.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tianlin.xyz/gtrhuqiqmz.html

Ruby: "ab" * 3
来源：http://hz.daxiang520.top/gtkkffswnn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258888.top/gtvyuthack.html

[E03] 截取子串
来源：http://hz.c1oappe.top/gttazrpqok.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yuxming.cn/gtptyfsmud.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tanke756.top/gtpofkrrrb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtyixuzhzn.html

TS:   s.slice(1, 4)
来源：http://hz.sysykeji.top/gtgrnfemnw.html

Java: s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtmpknozmz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shangyingyoupin.top/gtwefflxan.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jlsjyb.cn/gttfspbndu.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtyorgwykj.html

[E04] 查找子串位置
来源：http://hz.meibo888.top/gtmghzubvo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhaomingkeji.xyz/gteazsuhic.html

PHP:  strpos($s, "x");
来源：http://hz.dashuyun.cn/gtnfkppoos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhoulong.xyz/gtgalznujz.html

TS:   s.indexOf("x")
来源：http://hz.xinyue.icu/gthbixznvv.html

Java: s.indexOf("x")
来源：http://hz.zhengqikj.top/gttmhqxhbn.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtsooexdcp.html

Ruby: s.index("x")
来源：http://hz.iojbl.cn/gttzloheyg.html

C#:   s.IndexOf("x")
来源：http://hz.smart0.xyz/gtmyehcqau.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cheryme.top/gtfxqlwtfx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jiagoushi.top/gtyhzujnde.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenlongwang.top/gtrhfklosq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gthvsmxwcv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jiagoushi.top/gtysrakdyn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtplgipunq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ehwqpu.com/gtmpokdkkc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.snrcjt.cn/gtwdvkqbrr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangdashe.top/gtkramqetl.html

[E06] 替换子串
来源：http://hz.yj20258.top/gtwlalairs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hysaishi.cn/gtcxrmssho.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.hongshengwenyu.top/gtiqdmsisq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtqnvplbcv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.pycfn.com/gtxaplplrb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtbostguaw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.redwolf501.top/gtfbnpwjlv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.andypj.xyz/gtkmwssjib.html

C#:   s.Replace("a", "b")
来源：http://hz.daxiang520.top/gtwnqdoiho.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtcbajbajc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhixingplan.top/gtqclrkurl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.daxiang520.top/gtunndillq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtnzalochc.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtybtzqjkb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shuidangran.top/gtmzecurtg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.c1oappe.top/gtamwzyyub.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtzragccyx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shangyingyoupin.top/gtovfimbml.html

[E08] 数组按分隔符合并
来源：http://hz.fengsongda.top/gtjpuuppqv.html

Py:   ",".join(items)
来源：http://hz.cdnleiting.top/gtqkorfaxu.html

PHP:  implode(",", $items);
来源：http://hz.daria6918.cn/gtshcmxyea.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtvnzgablr.html

TS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtmmjxirvw.html

Java: String.join(",", items)
来源：http://hz.cashguo.top/gtmhkcpsdn.html

Go:   strings.Join(items, ",")
来源：http://hz.aizwys.cn/gtomamdeoh.html

Ruby: items.join(",")
来源：http://hz.zhixingplan.top/gtgcfqrfeq.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gttxttjaip.html

[E09] 去除所有空白字符
来源：http://hz.0kj1m.cn/gtwajsntxb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.c1oappe.top/gtyyzedhhc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xylfe.cn/gtzymldstu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yangfankeji.com/gtjzlfftdl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtlmsgxgql.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtujcovanv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhoulong.xyz/gtgcosoewj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.fengsongda.top/gtdxpjhevq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yj20258888.top/gtrodhfslv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yuxming.cn/gtqsswdpcu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuanzx.com/gttttcmscp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj202588.top/gtqkbavtlh.html

JS:   "7".padStart(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtczcjwamy.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtvujecfgh.html

Java: String.format("%03d", 7)
来源：http://hz.zhixingplan.top/gtmqxwyfbd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.nanxuanxn.top/gtrkkmlffz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cashguo.top/gtscjlgtjo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jqgfzy.top/gtxbnfpels.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtxfuxdfkd.html

Py:   s[::-1]
来源：http://hz.jinqigfzy.top/gtkhhmgxsp.html

PHP:  strrev($s);
来源：http://hz.yvedp.cn/gtkkgroiyk.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtwxmqxjul.html

TS:   [...s].reverse().join("")
来源：http://hz.jlsjyb.cn/gtexujzfvh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtbzjlflwq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yangfankeji.com/gtnbqodfbe.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtlbayjxeo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.daria6918.cn/gtnpuzrcye.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtcafrniqd.html

Py:   s.count("a")
来源：http://hz.gaohongyu789.top/gtxtcbntdj.html

PHP:  substr_count($s, "a");
来源：http://hz.smart0.xyz/gtkrgaahui.html

JS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtxynjunel.html

TS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gttskrbjyw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.gzhubu.top/gtntkccdnp.html

Go:   strings.Count(s, "a")
来源：http://hz.ehwqpu.com/gtncepmsnn.html

Ruby: s.count("a")
来源：http://hz.wangdashe.top/gtqdbhncjt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.9152youxi.cn/gtyyidzlyk.html

[E13] 逐字符遍历
来源：http://hz.hfpthk.cn/gtrradyhzg.html

Py:   for ch in s: print(ch)
来源：http://hz.pengpengdd.cyou/gtrwcksqmr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gtdnkxkqeu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtocpdfxbz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.gzhubu.top/gtmpfoiccd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ppjwa.cn/gtxqpofxke.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtzeutzqtj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ehwqpu.com/gtruatksnf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sweek.top/gtpjpewtln.html

[E14] URL 编码与 Base64
来源：http://hz.gogol.net.cn/gtkitldumf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtbmkzmfsf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gtlroddjln.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.c1oappe.top/gthakclzcw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.316326.xyz/gtaokfbzpq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gtlpmjawjz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.andypj.xyz/gtqzokvlyf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tianlin.xyz/gtomclcoqr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.guowangkeji.top/gtrvbrbphf.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenzaomai.com/gtjgnadlwt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gteihjechf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtqmbzwdss.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yanxiufei.cn/gtbbgljqcv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jyoumei.cn/gtmqjemtzy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.chenzaomai.com/gtfztomghn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xinyue.icu/gtttfqdmnx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtqqoewich.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zdqjudy.top/gtsfzialbf.html

[E16] 数字千分位
来源：http://hz.meibo888.top/gtzmktdhcz.html

Py:   f"{1234567:,}"
来源：http://hz.xingfuxueyuan.xyz/gtcpyhoctb.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtofgurtdd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigfzy.top/gtbcqcyfmz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.haohaochexian.top/gtbepicddd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xylfe.cn/gtampgoxsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.feifeiyinyue.top/gtfheayklv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtqktaetgq.html

C#:   1234567.ToString("N0")
来源：http://hz.ppjwa.cn/gtqaxqyzfz.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gtmuexocjg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.snrcjt.cn/gtrkfxmnyd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtwyutlduo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhengqikj.top/gteuknqkor.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtausvdmxu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gteeukfnac.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cdnleiting.top/gtwfzhsern.html

Ruby: s.capitalize
来源：http://hz.fengsongda.top/gtvkjpyytn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tanke756.top/gtwamtyzqk.html

[E18] 模板占位符替换
来源：http://hz.dianchejie.cn/gtksudkylg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtfyahjbpi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guowangkeji.top/gtngycsvcs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtshlevdpb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gotoacloud.top/gtiipcgamv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhoulong.xyz/gtdfefdbah.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xylfe.cn/gtnjcxdhoa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.bjfxy.top/gtmebwcqwm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnqzz.top/gtecjzljwl.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtegiiyzvn.html

Py:   s.splitlines()
来源：http://hz.tianlin.xyz/gtjwtpqwli.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.chenjidiqi.icu/gtiobtqred.html

JS:   s.split(/\r?\n/)
来源：http://hz.tanke756.top/gtastbkiau.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtaqgzwunh.html

Java: s.lines().toList()
来源：http://hz.xinyue.icu/gtklkxoqye.html

Go:   strings.Split(s, "\n")
来源：http://hz.yueranfly.top/gtufskfgxr.html

Ruby: s.lines
来源：http://hz.chenlongwang.top/gtkskbyspf.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gtekoabzha.html

[E20] 判断字符串是否为空
来源：http://hz.nwbrower.top/gtsdxnqkiy.html

Py:   if not s:
来源：http://hz.smart0.xyz/gtxsrdhgzh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtgihqzdlk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jiagoushi.top/gtwdctkwkf.html

TS:   if (s === "") {}
来源：http://hz.meibo888.top/gthgezfsti.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenzaomai.com/gtpeezvdsc.html

Go:   if s == "" {}
来源：http://hz.zhengqikj.top/gtevhjsgww.html

Ruby: if s.empty?
来源：http://hz.hongshengwenyu.top/gtigzwqtqo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gthzqjryqr.html

[E21] 超长截断加省略号
来源：http://hz.snrcjt.cn/gtehiidrnp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtsrqxifpl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.wangshuangyany.cn/gtxzgtqibx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xylfe.cn/gtjxhmpdju.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xziqi.cn/gtslrbzcbv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtywsqynyx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.andypj.xyz/gtcnhwmsqh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shuidangran.top/gtdxzcjqhn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.cqqwz.cn/gtkdyntueo.html

[E22] 字节长度与字符长度
来源：http://hz.hnqzz.top/gtotrhghfq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yangfankeji.com/gtcwvoztrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.haohaochexian.top/gtbkznmyei.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shzxlz.cn/gtdalcsklj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhengqikj.top/gtnzsurioa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtfyvpfkwe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtxyjxmhtg.html

Ruby: s.bytesize;  s.length
来源：http://hz.c1oappe.top/gtersqvofz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gtzzwxrrsf.html

================================================================================
来源：http://hz.cheryme.top/gtygololwb.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtlmgjbwkf.html

================================================================================
来源：http://hz.ehwqpu.com/gtofarjytg.html

[F01] 读取整个文件
来源：http://hz.c1oappe.top/gtpccsuhyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.shanyushiyangkeji.top/gtizjyubok.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gogol.net.cn/gtsrtdtoee.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.cqqwz.cn/gtszvtjkvz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.wangdashe.top/gtjzhmkahp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtbzbxywgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pengpengdd.cyou/gtemkcnyzm.html

Ruby: File.read("a.txt")
来源：http://hz.ydzc1.top/gttgqegknq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fengsongda.top/gtjsjdbnsw.html

[F02] 逐行读取文件
来源：http://hz.xylfe.cn/gtwswsqctc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.iojbl.cn/gtvnlaqcza.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.pycfn.com/gtjrtfsint.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtthecnkdb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gtqwiopynu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtnwmiuhfo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sweek.top/gtpgqobhtf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.chenjidiqi.icu/gtcowavbuy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtthroeqfv.html

[F03] 写入文件（覆盖）
来源：http://hz.zhiwuduotai.top/gtvdudskzo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shanyushiyangtech.top/gtzqducaeh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tian-w.cn/gtolhqocdt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtbfqrqvsc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtdipgqolh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.hfpthk.cn/gtlvuxtlon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xinyue.icu/gtwqcvigpb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxinkj.top/gtspxywezq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtxeyxcbcw.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gtzgawxzpd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.9152youxi.cn/gtrphubqmi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnxiangtu.top/gtqojimbuv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtczcohhmz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ppjwa.cn/gtjclngzbk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jiagoushi.top/gtwhtcyofk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.birdmap.top/gtpcziysvf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cucudq.cn/gtnfqijajl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ppjwa.cn/gtdhwlmujl.html

[F05] 判断文件或目录是否存在
来源：http://hz.gotoacloud.top/gtwhiisckk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tanke756.top/gtjxsprodn.html

PHP:  file_exists("a.txt");
来源：http://hz.tanke756.top/gtilhbrien.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gteowwfhis.html


<!-- 参考信息 -->