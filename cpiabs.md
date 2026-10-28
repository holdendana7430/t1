代发 wailian999

PHP:  in_array($x, $arr, true);
来源：http://hz.jlsjyb.cn/gtrnsdenbd.html

JS:   arr.includes(x)
来源：http://hz.meibo888.top/gtbcojazaj.html

TS:   arr.includes(x)
来源：http://hz.hammf.cn/gtgixaplvc.html

Java: list.contains(x)
来源：http://hz.yj202588.top/gtkizkmwcf.html

Go:   slices.Contains(arr, x)
来源：http://hz.guowangkeji.top/gtfiptavyf.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtjmpyarbi.html

C#:   list.Contains(x)
来源：http://hz.jinqigufen.top/gtbskygrlf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigfzy.top/gtrrqbpryn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtuusknxkp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gogol.net.cn/gtcudtddsj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtdohbixki.html

TS:   [...arr];
来源：http://hz.jyoumei.cn/gtnfubjtjh.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtpaiyiwwp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jlsjyb.cn/gtepwyshgj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtszwokgfl.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtfiylayyx.html

[D23] reduce 累积计算
来源：http://hz.shuidangran.top/gtluiajpxl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gtdtnvolji.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aibaodan.cn/gtxfyhofbo.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gogol.net.cn/gtikrwprlp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtvtqzttvm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtqgrsyuup.html

Go:   // 手写循环
来源：http://hz.nwbrower.top/gtylnvcqzs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hfpthk.cn/gtncvhyrdt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258.top/gtirszjijy.html

[D24] 字典 / Map 基本操作
来源：http://hz.daria6918.cn/gtocyxyiya.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtinclofiq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.redwolf501.top/gtbnfqeejd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtwsmrnxwo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.guowangkeji.top/gtkyqmdzuo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtwjzqiiia.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinqigufen.top/gtshpaxysj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.52xcode.cn/gtwktfyhuq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yueranfly.top/gtbhscwhzv.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtvplwmnaq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtlbohnzoi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.kuanghao11.cn/gtnblxzjcm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hnxiangtu.top/gttyzocayw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.nanxinkj.top/gtinhammtr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gtypukrikj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtbgpanlnf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cdnleiting.top/gtzyvigdaj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxinkj.top/gtrioazztb.html

[D26] 数组转字符串
来源：http://hz.yueranfly.top/gtsqekukbe.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gthyvlrlma.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtnjjxymkp.html

JS:   arr.join(", ")
来源：http://hz.gogol.net.cn/gtyhtuhyyk.html

TS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gttcrjwvuc.html

Java: String.join(", ", list)
来源：http://hz.316326.xyz/gtsfdyytnp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.iojbl.cn/gthiygjmfv.html

Ruby: arr.join(", ")
来源：http://hz.xinyue.icu/gtdyuietri.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtdpjgdxle.html

================================================================================
来源：http://hz.yangfankeji.com/gtkjrhuyzm.html

E. 字符串处理
来源：http://hz.gaohongyu789.top/gttprnglda.html

================================================================================
来源：http://hz.wangdashe.top/gtcivenorh.html

[E01] 拼接字符串
来源：http://hz.gogol.net.cn/gtklzmxhxp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtnlmengjs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxinkj.top/gtkyliddgt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtcfrytqpm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gtcgxwctdd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sysykeji.top/gtathbqync.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jyoumei.cn/gtrygkiaav.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jlsjyb.cn/gtnwicqufg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nwbrower.top/gtzrrfqbxr.html

[E02] 重复字符串
来源：http://hz.ydjk.org.cn/gtpkhwyqyu.html

Py:   "ab" * 3
来源：http://hz.havefunace.top/gtbvdrxdeh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtthverlii.html

JS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtmbunptdp.html

TS:   "ab".repeat(3)
来源：http://hz.sweek.top/gtppznzqcr.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtmzfcrktj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gtpkvupjti.html

Ruby: "ab" * 3
来源：http://hz.zhongyouzk.top/gtvcipsiwo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cashguo.top/gtremnoulu.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtezlinzfl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtyuhuxrib.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtjmzpdqpg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.52xcode.cn/gtmtsvdxxp.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtdyqgyode.html

Java: s.substring(1, 4)
来源：http://hz.cheryme.top/gtwebteiod.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.daria6918.cn/gtgbiechmb.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dianchejie.cn/gtauilirqe.html

C#:   s.Substring(1, 3)
来源：http://hz.52xcode.cn/gtswkcnzub.html

[E04] 查找子串位置
来源：http://hz.hongshengwenyu.top/gttriyxnzq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cashguo.top/gtdustklzm.html

PHP:  strpos($s, "x");
来源：http://hz.xinyue.icu/gtgzbaisdm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.svipenyu.cn/gtkfqqfbgj.html

TS:   s.indexOf("x")
来源：http://hz.smart0.xyz/gtdihiqjib.html

Java: s.indexOf("x")
来源：http://hz.hywenlv.cn/gthnuqrvtw.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gtfhwufnlx.html

Ruby: s.index("x")
来源：http://hz.cheryme.top/gtwchdbgxy.html

C#:   s.IndexOf("x")
来源：http://hz.ehwqpu.com/gtodukqfec.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yueranfly.top/gtptoulmfq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yangfankeji.com/gtdjmdpbjm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yongpay.top/gtxlqmvjbv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtejtdeywn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.haohaochexian.top/gtqkmonakj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtzjmjuvff.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhaomingkeji.xyz/gttoixvyas.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuetiantiany.cn/gtqmvkntkj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.wangshuangyany.cn/gtiujwohuj.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtprxfrwoc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258888.top/gttiuxqszf.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.chenzaomai.com/gtkqdalqug.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtyeawgdjg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtvvpwewzg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtgqxxrxkj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cucudq.cn/gtztdvibur.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cucudq.cn/gtzuqhxbgz.html

C#:   s.Replace("a", "b")
来源：http://hz.hysaishi.cn/gtvfogpumy.html

[E07] 按分隔符拆分
来源：http://hz.redwolf501.top/gtkpzogpcp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtppgzrnlz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hysaishi.cn/gtcptfzjcs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtdnseqshl.html

TS:   s.split(",")
来源：http://hz.gaohongyu789.top/gtlgymynbl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.wangshuangyany.cn/gtkquhjciq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.shanyushiyangkeji.top/gtaepmammt.html

Ruby: s.split(",");  s.split
来源：http://hz.cucudq.cn/gtmxkkcbew.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ivvv.top/gtlczgfghq.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtglfwbpxl.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtehojsyhn.html

PHP:  implode(",", $items);
来源：http://hz.wangdashe.top/gtbvyhmirk.html

JS:   items.join(",")
来源：http://hz.yonumen.top/gtglspjwed.html

TS:   items.join(",")
来源：http://hz.316326.xyz/gtdttmvpls.html

Java: String.join(",", items)
来源：http://hz.mhx1999.top/gtganlinhh.html

Go:   strings.Join(items, ",")
来源：http://hz.xziqi.cn/gttnoktvhi.html

Ruby: items.join(",")
来源：http://hz.zhengqikj.top/gteahfycck.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gtdffnsico.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gttawabwpb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jqgufenzy.top/gtmgzvlrkl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hywenlv.cn/gtejjzvhzd.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtyckipfon.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jyoumei.cn/gtexvlplpb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.redwolf501.top/gtdzrqbskb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuetiantiany.cn/gtbnmceqaj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinghuilouyu.cn/gtbyrwamih.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtgucuksij.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gturnnooxb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtpujhezsw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtqhuypdrv.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtsegxzpvi.html

TS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtkleqhyrl.html

Java: String.format("%03d", 7)
来源：http://hz.sweek.top/gtcqsorsql.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtevckzsmb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.aizwys.cn/gttstoodyw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tanke756.top/gtallmwnqz.html

[E11] 反转字符串
来源：http://hz.yongpay.top/gtftflzvrp.html

Py:   s[::-1]
来源：http://hz.sweek.top/gtqtaubbdt.html

PHP:  strrev($s);
来源：http://hz.xinyue.icu/gtgvhdosis.html

JS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtexotcziu.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gttydudbnl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shangyingyoupin.top/gtdmawapeq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sufxvd.cn/gtbcdqgksy.html

Ruby: s.reverse
来源：http://hz.yuxming.cn/gtasbyxgdy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.9152youxi.cn/gtcmkqnruz.html

[E12] 统计某字符出现次数
来源：http://hz.ppjwa.cn/gtvlhujmmn.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtmfvgjbck.html

PHP:  substr_count($s, "a");
来源：http://hz.gotoacloud.top/gtyangiawp.html

JS:   s.split("a").length - 1
来源：http://hz.hnqzz.top/gtzcigrder.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtortnszfc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.wangdashe.top/gtsiaymhbw.html

Go:   strings.Count(s, "a")
来源：http://hz.yongpay.top/gtbtkdlenu.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gttchtlsbb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnxiangtu.top/gticmjrbfd.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtjjxtbajv.html

Py:   for ch in s: print(ch)
来源：http://hz.ppjwa.cn/gtwfqfildl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtwmytgqzr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.52xcode.cn/gtueudeycz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtuffsbwls.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhixingplan.top/gttqzndfpf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinghuilouyu.cn/gtdnwwyiyy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.pengpengdd.cyou/gtjjfdbncf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuetiantiany.cn/gtummukhkd.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gtfmvwiaqg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtnrixfssz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.iojbl.cn/gtelataoly.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.gogol.net.cn/gtkpoayetp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtaxhnhglr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangdashe.top/gtepknakvs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.sxryk.cn/gtyynopkxa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxinkj.top/gtzkovowip.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtdnqjgtdc.html

[E15] HTML 转义 / 反转义
来源：http://hz.ydjk.org.cn/gtpdxwtqqd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.fengsongda.top/gtotifeziv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenzaomai.com/gtxggmpffk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yangfankeji.com/gttwrmnaih.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.52xcode.cn/gtpcddxqfi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daria6918.cn/gtoicwrwfp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenlongwang.top/gtfbszdqgz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ehwqpu.com/gtjxpyncrx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtoaivyrqd.html

[E16] 数字千分位
来源：http://hz.iojbl.cn/gtjfyixqbk.html

Py:   f"{1234567:,}"
来源：http://hz.jinqigfzy.top/gtgvgdldln.html

PHP:  number_format(1234567);
来源：http://hz.9152youxi.cn/gtzwaduwzv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gttduptgoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gthvlkjyft.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guannengcc.top/gtiestowfj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.zhaomingkeji.xyz/gtafzhdnmd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jiagoushi.top/gteebwkupl.html

C#:   1234567.ToString("N0")
来源：http://hz.quarkkingdee.top/gtfqvavqqh.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtqxiegnkp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hammf.cn/gtnhfeuqqt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.316326.xyz/gtikqajvzp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtbswcvphn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtctlyktyd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cdnleiting.top/gtaaktqfac.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.hysaishi.cn/gtnshjumaf.html

Ruby: s.capitalize
来源：http://hz.ybcxt.top/gtlnhcdddf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xziqi.cn/gtxofufocn.html

[E18] 模板占位符替换
来源：http://hz.andypj.xyz/gtuqdkzjla.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.tian-w.cn/gthafnwifd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sweek.top/gtaeabxjtq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jyoumei.cn/gtecundabz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.sysykeji.top/gtfpjfcpbb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtofaguoxs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jiagoushi.top/gtweiasvms.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xziqi.cn/gtuomkjtpx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xingfuxueyuan.xyz/gthwqfnrim.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtiapebwio.html

Py:   s.splitlines()
来源：http://hz.316326.xyz/gtjpfcrlqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.316326.xyz/gtjnfoznip.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtjyfzlzyh.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gtgasokpre.html

Java: s.lines().toList()
来源：http://hz.cashguo.top/gtxnnbnjtw.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtiyqhnrop.html

Ruby: s.lines
来源：http://hz.c1oappe.top/gtnluktfkc.html

C#:   s.Split('\n')
来源：http://hz.zhengqikj.top/gtqoaxiobc.html

[E20] 判断字符串是否为空
来源：http://hz.yanxiufei.cn/gtvsdcvcbc.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gthsandxrb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuanzhike.top/gtqheojtss.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yvedp.cn/gtisfewjrf.html

TS:   if (s === "") {}
来源：http://hz.nanxinkj.top/gturxqzjen.html

Java: if (s.isEmpty()) {}
来源：http://hz.mhx1999.top/gthzlcawll.html

Go:   if s == "" {}
来源：http://hz.shuidangran.top/gtkcjzdhsf.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtmzuqjynl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.wangdashe.top/gttzarvtbt.html

[E21] 超长截断加省略号
来源：http://hz.nanxuanxn.top/gttxflceil.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nwbrower.top/gtxnwrzctx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.nanxinkj.top/gtxbvcuduh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtvfsknlmd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.vqdsnc.cn/gteuvxorkz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtymzxmvdo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cashguo.top/gtdnoxjpyu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gtzivscdil.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yanxiufei.cn/gtfngupebt.html

[E22] 字节长度与字符长度
来源：http://hz.quarkkingdee.top/gttghvzkvj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.fzhhl.top/gtaiakwrnn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtsbopioif.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ybcxt.top/gtaijkzwlw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.fengsongda.top/gtxyzvjjxt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtpjzrvqhh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.xingfuxueyuan.xyz/gtjnpyrilm.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtvwjhkohn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yvedp.cn/gtltpgcngn.html

================================================================================
来源：http://hz.mhx1999.top/gtcxmpasyc.html

F. 文件与目录
来源：http://hz.zhengqikj.top/gtxmafvtjl.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlvuflots.html

[F01] 读取整个文件
来源：http://hz.cucudq.cn/gthshxvfqo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.nanxinkj.top/gtwcrlpqqt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pengpengdd.cyou/gtqarkakvb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.tianlin.xyz/gtlgfreqjs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.pycfn.com/gturqakzis.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj20258.top/gtednbwtwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.guowangkeji.top/gtraucyvkh.html

Ruby: File.read("a.txt")
来源：http://hz.hfpthk.cn/gthuzhyixr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhoulong.xyz/gtdorwamlt.html

[F02] 逐行读取文件
来源：http://hz.shangyingyoupin.top/gtanrlfvnd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhiwuduotai.top/gtjlxypxxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gogol.net.cn/gtjbswzqio.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtkzryfulk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pycfn.com/gthpirjtsd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.shuidangran.top/gtzjcmsynd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtvokffdip.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hnxiangtu.top/gteaxogxwh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tian-w.cn/gttiawtqyn.html

[F03] 写入文件（覆盖）
来源：http://hz.shanyushiyangkeji.top/gtgvbcdagj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.daria6918.cn/gtoxzrqnzu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtjhekvrlk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gthxcyknlv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.smart0.xyz/gtuibcssgi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxinkj.top/gtqowfgbwb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinyuanbaomall.cn/gtdzkhfacr.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtmjjdimht.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtjfqkbwhs.html

[F04] 追加写入文件
来源：http://hz.dashuyun.cn/gtdlqatzdq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hongshengwenyu.top/gtimzkrcrd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hongshengwenyu.top/gtsorkztrq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtcgjiogeq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hammf.cn/gtynmogzch.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xinyue.icu/gtqpinsgpk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.aizwys.cn/gtvckyopot.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.redwolf501.top/gteadbmipe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yueranfly.top/gtrrtfhajc.html

[F05] 判断文件或目录是否存在
来源：http://hz.dashuyun.cn/gtcqrlbsrm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258.top/gtrfdnspig.html

PHP:  file_exists("a.txt");
来源：http://hz.birdmap.top/gtkinzrvkf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtyjwsmedr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gthwmtvngp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtcckyhuwx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.iojbl.cn/gtogjhxzhh.html

Ruby: File.exist?("a.txt")
来源：http://hz.ydjk.org.cn/gtmysmzoxe.html


<!-- 参考信息 -->