代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://hz.yanxiufei.cn/gtwclvcmlw.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtizmcbxkq.html

C#:   list.Contains(x)
来源：http://hz.chenlongwang.top/gtqogetyqx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhixingplan.top/gtntpysajn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtkbujevvy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sufxvd.cn/gtrcdygpha.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenjidiqi.icu/gtyvmhbldf.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtgxbqeugi.html

Java: new ArrayList<>(list);
来源：http://hz.bjfxy.top/gtihkqxhba.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hnqzz.top/gttchvphuc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hammf.cn/gtvpxicvhl.html

C#:   new List<int>(list);
来源：http://hz.daxiang520.top/gteeqexqjn.html

[D23] reduce 累积计算
来源：http://hz.xinyue.icu/gtbbimdpkq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.andypj.xyz/gtezwvrqow.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nwbrower.top/gtdepjnzlz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.andypj.xyz/gtcywmflpa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtunlvaszd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nanxuanxn.top/gtljxphmvn.html

Go:   // 手写循环
来源：http://hz.aizwys.cn/gtzexilbim.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jiagoushi.top/gtqvadryyd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtccylnlrg.html

[D24] 字典 / Map 基本操作
来源：http://hz.nanxuanxn.top/gttljnyhah.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xinyue.icu/gtifizwabo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tianlin.xyz/gtvinweimy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yueranfly.top/gtlpwwpnvh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.meibo888.top/gtvgjdelsg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtlsprdavh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zdqjudy.top/gtnonxaegq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtupqckxir.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gttflyiiux.html

[D25] Set 集合去重与交并差
来源：http://hz.tanke756.top/gtqwwhycfl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtqcfjfkrp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yangfankeji.com/gtdpdgahzx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtcoiladmz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.tanke756.top/gtysuswkrj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtfdyfilxj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxinkj.top/gtqbcvyfdt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ivvv.top/gtsnmznwmq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.feifeiyinyue.top/gtgzbumtls.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtvykxpcme.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinqigufen.top/gtacqnjcsz.html

PHP:  implode(", ", $arr);
来源：http://hz.hfpthk.cn/gtafuupdlt.html

JS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtifymjphi.html

TS:   arr.join(", ")
来源：http://hz.havefunace.top/gtthfivgmh.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtaguxwhwc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtvrtrlzvw.html

Ruby: arr.join(", ")
来源：http://hz.jinyuanbaomall.cn/gtifpynbex.html

C#:   string.Join(", ", list)
来源：http://hz.pycfn.com/gtkeauigfx.html

================================================================================
来源：http://hz.kuanghao11.cn/gtvxygojpo.html

E. 字符串处理
来源：http://hz.ydjk.org.cn/gthjfuqxba.html

================================================================================
来源：http://hz.yangfankeji.com/gtdtokghoo.html

[E01] 拼接字符串
来源：http://hz.meibo888.top/gtkufxmqhz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yangfankeji.com/gtfbptbatk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gaohongyu789.top/gtjzvwziae.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtdfrbgikl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtrrhugfaj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guannengcc.top/gtfithzytt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ywan-chungtsiang.top/gteoxytdxf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhaomingkeji.xyz/gtsavbxydo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtrbnlvztk.html

[E02] 重复字符串
来源：http://hz.ywan-chungtsiang.top/gtwxqedqdr.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gthycugnbf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhaomingkeji.xyz/gtjxnqzpml.html

JS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtkipwlmil.html

TS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gtxodlpasm.html

Java: "ab".repeat(3)
来源：http://hz.nwbrower.top/gtpclkeiiq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtqbalnnmm.html

Ruby: "ab" * 3
来源：http://hz.gogol.net.cn/gthlewiaao.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtrbvzivvc.html

[E03] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtcoaufdwm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ybcxt.top/gtaermqios.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cucudq.cn/gtmxwukkqr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtyqtkwlxy.html

TS:   s.slice(1, 4)
来源：http://hz.yj202588.top/gtzrbnssvs.html

Java: s.substring(1, 4)
来源：http://hz.yongpay.top/gtqaiytdfw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jlsjyb.cn/gtlagzcuyk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.daxiang520.top/gtwzlacazi.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gtaskfghfq.html

[E04] 查找子串位置
来源：http://hz.chenjidiqi.icu/gtfhgqvinr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtiwfaittl.html

PHP:  strpos($s, "x");
来源：http://hz.sysykeji.top/gtajjceppp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtjfruxmuy.html

TS:   s.indexOf("x")
来源：http://hz.feifeiyinyue.top/gtcyuuusuc.html

Java: s.indexOf("x")
来源：http://hz.ydzc1.top/gtezmqqceo.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtpwrdkzwq.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtorpgygpu.html

C#:   s.IndexOf("x")
来源：http://hz.zhijiandao.cn/gtxjxityar.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gttgkcwdat.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gtsublqhab.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhiwuduotai.top/gtuuzgtwzw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtweguhing.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yuxming.cn/gtjmxfrspd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ppjwa.cn/gtetvohlne.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.kuanghao11.cn/gtegxuzpje.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtigfajvex.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenlongwang.top/gthhgvhbpg.html

[E06] 替换子串
来源：http://hz.shangyingyoupin.top/gtfydsnpqf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xylfe.cn/gtgldjfpur.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xingfuxueyuan.xyz/gtrawzvpxx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ivvv.top/gtxtnzxpwf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtnliwxpcv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtryxjjmim.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhoulong.xyz/gtncnnxdxu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xziqi.cn/gtjffmmrot.html

C#:   s.Replace("a", "b")
来源：http://hz.gzhubu.top/gtsruqxjua.html

[E07] 按分隔符拆分
来源：http://hz.tianlin.xyz/gtwgqyviyr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtnanjqgjk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.kuanghao11.cn/gtmhvzonlu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gtpinefwpn.html

TS:   s.split(",")
来源：http://hz.guannengcc.top/gtigygmqxg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xingfuxueyuan.xyz/gtbebpxryo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtuhevfnwk.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtibudiqph.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.0kj1m.cn/gtmynplelk.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtbrmhaewg.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtghvrndsb.html

PHP:  implode(",", $items);
来源：http://hz.quarkkingdee.top/gtnfcfluyd.html

JS:   items.join(",")
来源：http://hz.zhiwuduotai.top/gtfoymoipa.html

TS:   items.join(",")
来源：http://hz.tianlin.xyz/gtsgnpfyoh.html

Java: String.join(",", items)
来源：http://hz.xziqi.cn/gtksaumqsi.html

Go:   strings.Join(items, ",")
来源：http://hz.yuanzhike.top/gtocsxorgo.html

Ruby: items.join(",")
来源：http://hz.xingfuxueyuan.xyz/gttonqcowp.html

C#:   string.Join(",", items)
来源：http://hz.birdmap.top/gtsyvmgskt.html

[E09] 去除所有空白字符
来源：http://hz.birdmap.top/gtehmkupfj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtzuwlkijt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.0kj1m.cn/gtsxkxjdkw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtvqmzuzxj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.ybcxt.top/gteysdlyoi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.c1oappe.top/gttnunmxir.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gtmbpobvfy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258.top/gtrgurjdmi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yongpay.top/gtviutvbmq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtigjukozq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigufen.top/gtvlxsxskr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtpyttajyu.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtixprllmn.html

TS:   "7".padStart(3, "0")
来源：http://hz.mhx1999.top/gtstrlhhbu.html

Java: String.format("%03d", 7)
来源：http://hz.fengsongda.top/gtfswrwuzq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hfpthk.cn/gtcxqfbzes.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xylfe.cn/gtlrvnwrii.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtbabiqbde.html

[E11] 反转字符串
来源：http://hz.feifeiyinyue.top/gtfaulxcqt.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtpopfsasx.html

PHP:  strrev($s);
来源：http://hz.zycfv.cn/gtklnsdvgr.html

JS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtqtlofkkw.html

TS:   [...s].reverse().join("")
来源：http://hz.dashuyun.cn/gtxqaoedtt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sufxvd.cn/gtaasxnmyb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xuetiantiany.cn/gtznqrbvvy.html

Ruby: s.reverse
来源：http://hz.andypj.xyz/gtqzetczqi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.gaohongyu789.top/gtzdgwzzkf.html

[E12] 统计某字符出现次数
来源：http://hz.jqgfzy.top/gthzqivboj.html

Py:   s.count("a")
来源：http://hz.316326.xyz/gtndlbnirr.html

PHP:  substr_count($s, "a");
来源：http://hz.cucudq.cn/gtxftnktqp.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtfmatyfty.html

TS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtxgvbyfpm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinqigufen.top/gtnobeeran.html

Go:   strings.Count(s, "a")
来源：http://hz.ybcxt.top/gtuoqqferq.html

Ruby: s.count("a")
来源：http://hz.meibo888.top/gtevxuaqpf.html

C#:   s.Count(c => c == 'a')
来源：http://hz.mhx1999.top/gtwbafobah.html

[E13] 逐字符遍历
来源：http://hz.shanyushiyangkeji.top/gtgumpzecn.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtokctyxah.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.vqdsnc.cn/gtpplxryyr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.birdmap.top/gtmqnqclue.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.316326.xyz/gtxzzuuehp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.quarkkingdee.top/gtechjeyzu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtgogeddvu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gogol.net.cn/gteiquaxcm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtjhawzlce.html

[E14] URL 编码与 Base64
来源：http://hz.yangfankeji.com/gttktlvrbz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gtxijqcjde.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.havefunace.top/gtffvxhvus.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yvedp.cn/gtvorurzwl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ehwqpu.com/gtirfekaen.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cheryme.top/gtrgjhkaxl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jlsjyb.cn/gtltnhnfrt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.tanke756.top/gtbeqrnmhp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtrejqvemk.html

[E15] HTML 转义 / 反转义
来源：http://hz.9152youxi.cn/gtmjiyplin.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigfzy.top/gtfmzceema.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtjtudmkxd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.andypj.xyz/gtholbgmhj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtxiqbxgvw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhongyouzk.top/gtuuwrywcu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtekvsgxhc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangdashe.top/gtvdskebvd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hywenlv.cn/gtdejaehgt.html

[E16] 数字千分位
来源：http://hz.cucudq.cn/gthwgwigzw.html

Py:   f"{1234567:,}"
来源：http://hz.sxryk.cn/gtijqdrcbb.html

PHP:  number_format(1234567);
来源：http://hz.vqdsnc.cn/gtreanzzjt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtteopweev.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtkfqmscgz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtuqztqjae.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinqigfzy.top/gtgwcfzmhm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtsegwxfqp.html

C#:   1234567.ToString("N0")
来源：http://hz.chenzaomai.com/gtmeohdrga.html

[E17] 首字母大写
来源：http://hz.birdmap.top/gtpbtuocfs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.gogol.net.cn/gtfydagarm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guannengcc.top/gtxosefrcx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtfuaoiooi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cdnleiting.top/gtooticbmv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtxyczrifa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gtcvbomltt.html

Ruby: s.capitalize
来源：http://hz.ppjwa.cn/gttjaasoqs.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtfgcrrmua.html

[E18] 模板占位符替换
来源：http://hz.xinyue.icu/gttfuuniuc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ybcxt.top/gtrafniuun.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.meibo888.top/gtfyfexwod.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtusnzsjia.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.meibo888.top/gtxptijtjv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.vqdsnc.cn/gtqygborwd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shzxlz.cn/gttkjzkteq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.andypj.xyz/gtjagdrtyq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gtymhkojfd.html

[E19] 多行文本按行拆分
来源：http://hz.chenjidiqi.icu/gteqfwdxui.html

Py:   s.splitlines()
来源：http://hz.mhx1999.top/gtmpmpimya.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.feifeiyinyue.top/gtpfwejigq.html

JS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtdjmumobo.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gttvqtgnhk.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gtwqlwxpyy.html

Go:   strings.Split(s, "\n")
来源：http://hz.yj20258.top/gtongkoozy.html

Ruby: s.lines
来源：http://hz.jqgfzy.top/gtyuhbeejw.html

C#:   s.Split('\n')
来源：http://hz.gzhubu.top/gtxgpkgsml.html

[E20] 判断字符串是否为空
来源：http://hz.meibo888.top/gtbzqesore.html

Py:   if not s:
来源：http://hz.ydjk.org.cn/gtmnsefpoy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ywan-chungtsiang.top/gtxvdizihq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.cdnleiting.top/gtzdeoaktl.html

TS:   if (s === "") {}
来源：http://hz.havefunace.top/gteplogvtl.html

Java: if (s.isEmpty()) {}
来源：http://hz.hongshengwenyu.top/gtkrcvajjk.html

Go:   if s == "" {}
来源：http://hz.cucudq.cn/gtbngdjmjc.html

Ruby: if s.empty?
来源：http://hz.shangyingyoupin.top/gtinziodnc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.haohaochexian.top/gtkhwplqsr.html

[E21] 超长截断加省略号
来源：http://hz.zhiwuduotai.top/gtdnscljuz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ywan-chungtsiang.top/gtalilitna.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jinqigufen.top/gtadqmjgfg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtbkxgwgvx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.52xcode.cn/gthjdjqkzi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtdajunweg.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtisdzqlko.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuanzx.com/gtfocjvhmz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtkrfwfyon.html

[E22] 字节长度与字符长度
来源：http://hz.snrcjt.cn/gtkpzuhqfp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zdqjudy.top/gtcpzplifd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hysaishi.cn/gtivuzxmsw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtcloptqbk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtdebhyikx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenjidiqi.icu/gtotisnayv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xylfe.cn/gtiepxknjz.html

Ruby: s.bytesize;  s.length
来源：http://hz.gogol.net.cn/gtfdcflqkx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pengpengdd.cyou/gtqbvfmrlw.html

================================================================================
来源：http://hz.yj20258.top/gtcrqoppqg.html

F. 文件与目录
来源：http://hz.gogol.net.cn/gtrrtgslij.html

================================================================================
来源：http://hz.c1oappe.top/gtovkcpwyj.html

[F01] 读取整个文件
来源：http://hz.0kj1m.cn/gtzxxnimgn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.hysaishi.cn/gtkxvmyhfo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtscknlhiw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.haohaochexian.top/gtskuputjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.snrcjt.cn/gtmamkjpbp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nwbrower.top/gtpyxcmhcx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.redwolf501.top/gtpaoczavp.html

Ruby: File.read("a.txt")
来源：http://hz.xuanzx.com/gtofmunzyh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yueranfly.top/gthnqkfzqq.html

[F02] 逐行读取文件
来源：http://hz.dianchejie.cn/gtyxaieidv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.meibo888.top/gtdoridhfk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sysykeji.top/gtgfouikff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtzycjnnml.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aizwys.cn/gtnesesxty.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtqnnntzhl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.shanyushiyangkeji.top/gtqnhxznar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.birdmap.top/gtflayeoqj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.svipenyu.cn/gtyqyyyvfu.html

[F03] 写入文件（覆盖）
来源：http://hz.guowangkeji.top/gtjdbqkppp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gtvppmclcl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinqigufen.top/gtduyjwujk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtjkfmkugu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gtjohhtygp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.guowangkeji.top/gtltqxdqoa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sweek.top/gtyayydcxx.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.xuanzx.com/gtvngrhojv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtwvazonix.html

[F04] 追加写入文件
来源：http://hz.fzhhl.top/gtuorpdbbj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.mhx1999.top/gtyrexveye.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.316326.xyz/gtnjprjycm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtqhwojdnu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtxanlopbm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhijiandao.cn/gtuokouenb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hfpthk.cn/gtjfbakycb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtnefxzovt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cdnleiting.top/gtbxpmpeqx.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtrfvihcwj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gttiqhbmqz.html

PHP:  file_exists("a.txt");
来源：http://hz.svipenyu.cn/gtnafrifuv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtkyizckza.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtglaaokwb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtithzkprg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gttigcdxdz.html

Ruby: File.exist?("a.txt")
来源：http://hz.svipenyu.cn/gtoqqlcnxs.html

C#:   File.Exists("a.txt")
来源：http://hz.yongpay.top/gtoebazfwa.html

[F06] 删除文件
来源：http://hz.tianlin.xyz/gtekfozsov.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gtbqkjkkgi.html

PHP:  unlink("a.txt");
来源：http://hz.sweek.top/gttzkrhzun.html


<!-- 参考信息 -->