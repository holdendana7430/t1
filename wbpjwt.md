代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.52xcode.cn/gtjrtjftnu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtyqdkkzlm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tianlin.xyz/gtivwhbdoi.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtnwdraphh.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gtnnvujqsh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuanzx.com/gtuxwabvxz.html

[D21] 判断是否包含某元素
来源：http://hz.xziqi.cn/gtuqclxbpj.html

Py:   x in arr
来源：http://hz.sweek.top/gtoxruonhw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtzohiepxs.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtxireqcsn.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtxrxczkuy.html

Java: list.contains(x)
来源：http://hz.hammf.cn/gtnafgrrtw.html

Go:   slices.Contains(arr, x)
来源：http://hz.wangdashe.top/gtuwadwkmv.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtlfecctap.html

C#:   list.Contains(x)
来源：http://hz.cashguo.top/gtdmubhjfl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sxryk.cn/gtrkwovpnj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shuidangran.top/gtuhknwyts.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhijiandao.cn/gtqcdakbjn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aizwys.cn/gtczefdzpd.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtirsntnny.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gteyynwbev.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gtaayyuvcw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtserxmfdq.html

C#:   new List<int>(list);
来源：http://hz.sweek.top/gtkkmtnvwk.html

[D23] reduce 累积计算
来源：http://hz.cheryme.top/gtinutccxh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fengsongda.top/gtillrsoak.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtzjchlako.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtiytambox.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtnpfqntqy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.sufxvd.cn/gtirspsijh.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gtrhuhckke.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gttwfidtpg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yonumen.top/gtqqghnhtg.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigfzy.top/gtjulkskpi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zdqjudy.top/gtkkwvsnbv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtphgwpexj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangtech.top/gtxofajwlt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtghvpxoei.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xuetiantiany.cn/gtttdkmbwi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cucudq.cn/gthyuzeavu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gtrtkcrjqq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.kuanghao11.cn/gtctsxddsm.html

[D25] Set 集合去重与交并差
来源：http://hz.dianchejie.cn/gtpazypsjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tianlin.xyz/gtsrbzfxzz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.svipenyu.cn/gtsgwhhsxz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.birdmap.top/gtvvahvrtd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xylfe.cn/gtimajsyvm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangshuangyany.cn/gtgupegequ.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinqigufen.top/gtrusrtzoo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinyuanbaomall.cn/gtgnesneul.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yvedp.cn/gtczgvrods.html

[D26] 数组转字符串
来源：http://hz.ydjk.org.cn/gtztmqnbjf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sysykeji.top/gttfokjswg.html

PHP:  implode(", ", $arr);
来源：http://hz.aizwys.cn/gtngtbehmv.html

JS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtvcghypwi.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtycjxuvtz.html

Java: String.join(", ", list)
来源：http://hz.chenlongwang.top/gtkvsyuybj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtlgzexbwg.html

Ruby: arr.join(", ")
来源：http://hz.meibo888.top/gtbguztzua.html

C#:   string.Join(", ", list)
来源：http://hz.cucudq.cn/gtjjitycvy.html

================================================================================
来源：http://hz.0kj1m.cn/gttswvegkl.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtowfvltat.html

================================================================================
来源：http://hz.9152youxi.cn/gtecfqwzrd.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtsyecczeq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtniazmxto.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aizwys.cn/gtorxbtlvx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.52xcode.cn/gtvuaixuki.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gthlcxuyvs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhongyouzk.top/gtsgdxqyhk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtfvisxibt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zdqjudy.top/gtqxwjrvqz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.aibaodan.cn/gtkyrvewhq.html

[E02] 重复字符串
来源：http://hz.guowangkeji.top/gtmaijlvjq.html

Py:   "ab" * 3
来源：http://hz.wangshuangyany.cn/gtyrzxptso.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aibaodan.cn/gtifnrnxmc.html

JS:   "ab".repeat(3)
来源：http://hz.meibo888.top/gthbhzpmez.html

TS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtpgyvrfpu.html

Java: "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gttfnkjbnf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hfpthk.cn/gtbocfptsc.html

Ruby: "ab" * 3
来源：http://hz.gaohongyu789.top/gtehdlelsp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangtech.top/gtmbebtthu.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtzzwnuzhj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtjprsmzhd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xinyue.icu/gtgncigwrx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtgpgwubhb.html

TS:   s.slice(1, 4)
来源：http://hz.zhixingplan.top/gtmkqwldmg.html

Java: s.substring(1, 4)
来源：http://hz.daria6918.cn/gtfbgsnfjw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtewfuswmm.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shuidangran.top/gtisjpttij.html

C#:   s.Substring(1, 3)
来源：http://hz.ydzc1.top/gtnfkdjuml.html

[E04] 查找子串位置
来源：http://hz.ybcxt.top/gtttiihyzt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.havefunace.top/gtgtwlwyor.html

PHP:  strpos($s, "x");
来源：http://hz.jiagoushi.top/gtzfetizck.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtsvflufku.html

TS:   s.indexOf("x")
来源：http://hz.cqqwz.cn/gtpacyaskl.html

Java: s.indexOf("x")
来源：http://hz.jqgfzy.top/gtowzucqbj.html

Go:   strings.Index(s, "x")
来源：http://hz.sweek.top/gtccornuvk.html

Ruby: s.index("x")
来源：http://hz.ywan-chungtsiang.top/gthtsekajq.html

C#:   s.IndexOf("x")
来源：http://hz.pengpengdd.cyou/gtujhknpie.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ybcxt.top/gtosailgro.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydjk.org.cn/gttmtigwoh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tanke756.top/gthuzjfeyb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtenvnszfm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtqjznytig.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtfhxzcfmg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhijiandao.cn/gtjskbubyc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aizwys.cn/gtuebunzdk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jyoumei.cn/gtnfjaeqha.html

[E06] 替换子串
来源：http://hz.yj20258.top/gturanajui.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gteeizwlol.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtisqvxiou.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yuxming.cn/gtlezllnmi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtzvvgnfdm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gthxnumxnw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.pycfn.com/gtsqqedpgz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gtcvnolygs.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtiynehbfw.html

[E07] 按分隔符拆分
来源：http://hz.9152youxi.cn/gtdhrczufo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yongpay.top/gtgcyxjgqh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jqgufenzy.top/gtnzpfgeia.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ywan-chungtsiang.top/gttvejaqox.html

TS:   s.split(",")
来源：http://hz.jyoumei.cn/gtmhgbvwex.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtpnboaknn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.sxryk.cn/gtimbnsite.html

Ruby: s.split(",");  s.split
来源：http://hz.xuanzx.com/gtvntzbepn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtekxxdxjg.html

[E08] 数组按分隔符合并
来源：http://hz.jianghu66.top/gtwlitueiw.html

Py:   ",".join(items)
来源：http://hz.aizwys.cn/gtphexezah.html

PHP:  implode(",", $items);
来源：http://hz.cheryme.top/gtdgnsianj.html

JS:   items.join(",")
来源：http://hz.ppjwa.cn/gtgqymewik.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtannwceej.html

Java: String.join(",", items)
来源：http://hz.shzxlz.cn/gtqajhlvmf.html

Go:   strings.Join(items, ",")
来源：http://hz.sufxvd.cn/gtcrpuziua.html

Ruby: items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtnhwntsdn.html

C#:   string.Join(",", items)
来源：http://hz.zycfv.cn/gtuezotfwt.html

[E09] 去除所有空白字符
来源：http://hz.wangdashe.top/gtfgbjhixb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sxryk.cn/gtaifzvdes.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.aizwys.cn/gtplhkkkbt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yj20258.top/gtqwvpbtwp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yuxming.cn/gtytjtuwin.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxinkj.top/gtolcwtaab.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pengpengdd.cyou/gtmepehzun.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtjprfralo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtajiwswri.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cdnleiting.top/gtoflgnmob.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtrpshekiu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jlsjyb.cn/gtxoxjictq.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtnsqunkwt.html

TS:   "7".padStart(3, "0")
来源：http://hz.vqdsnc.cn/gtfdxchrgl.html

Java: String.format("%03d", 7)
来源：http://hz.cqqwz.cn/gtjopmcjlc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtpkvcscxi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cheryme.top/gtmnxnozkm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fzhhl.top/gtqedppmwb.html

[E11] 反转字符串
来源：http://hz.yonumen.top/gtbtveaejl.html

Py:   s[::-1]
来源：http://hz.jqgfzy.top/gtmkofuthg.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gtgzepcdiu.html

JS:   [...s].reverse().join("")
来源：http://hz.gaohongyu789.top/gtinoqprut.html

TS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtgznjjhje.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydjk.org.cn/gtwdkyjauk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtlrporolt.html

Ruby: s.reverse
来源：http://hz.chenzaomai.com/gtfrkvagay.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hnxiangtu.top/gtpgbtilnd.html

[E12] 统计某字符出现次数
来源：http://hz.316326.xyz/gtrqihvlre.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtynjbbwsq.html

PHP:  substr_count($s, "a");
来源：http://hz.pengpengdd.cyou/gtcczaqljt.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtcfoqtzhi.html

TS:   s.split("a").length - 1
来源：http://hz.hywenlv.cn/gtpckonitg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hysaishi.cn/gtgrhjpwkt.html

Go:   strings.Count(s, "a")
来源：http://hz.jyoumei.cn/gttjxjlilz.html

Ruby: s.count("a")
来源：http://hz.quarkkingdee.top/gtitumfquw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuanzhike.top/gtrewifqcm.html

[E13] 逐字符遍历
来源：http://hz.chenjidiqi.icu/gtlljyjfdn.html

Py:   for ch in s: print(ch)
来源：http://hz.jqgufenzy.top/gtlvtbelrs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.iojbl.cn/gtreosgkur.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtgkojyhqh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtkjwlgbuu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shanyushiyangkeji.top/gttbzpadsl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhengqikj.top/gtgrgzocky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gogol.net.cn/gtmdnxiktp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangshuangyany.cn/gtrzyujasy.html

[E14] URL 编码与 Base64
来源：http://hz.yvedp.cn/gtgbwvmhwt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hnqzz.top/gtlmwteagb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtcqxmpwsy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.fengsongda.top/gttslnikio.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtaqzuqsvm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aizwys.cn/gtsuacinvx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ydjk.org.cn/gtdmcszufl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtlrictezh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shanyushiyangkeji.top/gtnezcnbfq.html

[E15] HTML 转义 / 反转义
来源：http://hz.daxiang520.top/gtmaorlqly.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.tian-w.cn/gttreivkzv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ppjwa.cn/gtpxabwgfk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtarvkgqqf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fengsongda.top/gtctvvlzpq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.andypj.xyz/gtzxmldwkb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jlsjyb.cn/gtlumqiyfv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.guowangkeji.top/gtuobkgseb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.birdmap.top/gtcgsydhsw.html

[E16] 数字千分位
来源：http://hz.yangfankeji.com/gtpbxrylql.html

Py:   f"{1234567:,}"
来源：http://hz.zhixingplan.top/gtjnrrkalq.html

PHP:  number_format(1234567);
来源：http://hz.haohaochexian.top/gtgqkrfcxo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gtfaoktvek.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gteojcnslv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.chenlongwang.top/gtnoaisipj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yvedp.cn/gtkwqyupkk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zdqjudy.top/gtzyjhevib.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtreltolqg.html

[E17] 首字母大写
来源：http://hz.aizwys.cn/gtfwjisapr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hfpthk.cn/gtathuvtsc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.9152youxi.cn/gtnlvdygtv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.kuanghao11.cn/gtisemxdmj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtivhmjmvn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.kuanghao11.cn/gtohukgqai.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dashuyun.cn/gttlcllttk.html

Ruby: s.capitalize
来源：http://hz.yj202588.top/gtbveqfqgj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cqqwz.cn/gtdszkhndy.html

[E18] 模板占位符替换
来源：http://hz.sxryk.cn/gtudzqmgmj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.52xcode.cn/gtpbxfhtnb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zycfv.cn/gtgknmbhhu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuanzx.com/gttuwjqqou.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtergzhcpb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.gotoacloud.top/gteplvnjah.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nanxinkj.top/gtckkqmpns.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.c1oappe.top/gtradyycuq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.shanyushiyangkeji.top/gtcxjgxwaw.html

[E19] 多行文本按行拆分
来源：http://hz.fzhhl.top/gtbcnnkhtm.html

Py:   s.splitlines()
来源：http://hz.yj20258888.top/gtjatwjroj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhiwuduotai.top/gtbduoqkqt.html

JS:   s.split(/\r?\n/)
来源：http://hz.iojbl.cn/gtkfxaheel.html

TS:   s.split(/\r?\n/)
来源：http://hz.aibaodan.cn/gtmjdwpogw.html

Java: s.lines().toList()
来源：http://hz.fzhhl.top/gtruhfvfrs.html

Go:   strings.Split(s, "\n")
来源：http://hz.hywenlv.cn/gtrpnckjxx.html

Ruby: s.lines
来源：http://hz.ivvv.top/gttoseurua.html

C#:   s.Split('\n')
来源：http://hz.pycfn.com/gtgynkwrvk.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gtqpjqmdcp.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gthrsgnboe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.ydjk.org.cn/gtiwhhuixg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.feifeiyinyue.top/gtjjsppivp.html

TS:   if (s === "") {}
来源：http://hz.yj20258888.top/gtyrowohvh.html

Java: if (s.isEmpty()) {}
来源：http://hz.dianchejie.cn/gtxfcdnnbs.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtzlynjyse.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtscvzmncw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtllxlzlce.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gtsdqnwbsm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yueranfly.top/gtckqoiybr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gtvavbaiqp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtswwdhobg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.guannengcc.top/gttrtzmool.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.hammf.cn/gttviyrdmy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cashguo.top/gtbaqsaqph.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.chenzaomai.com/gtfuihgfog.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gthbuwrkuf.html

[E22] 字节长度与字符长度
来源：http://hz.zdqjudy.top/gtuewhmlyw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gtgthdxiab.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.redwolf501.top/gthqnhuubx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtbxgeyacq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cashguo.top/gtewtpouva.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.redwolf501.top/gtsmsimduj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtgzwgqbud.html

Ruby: s.bytesize;  s.length
来源：http://hz.kuanghao11.cn/gtzknbgkwa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shzxlz.cn/gtxpvetuex.html

================================================================================
来源：http://hz.snrcjt.cn/gttpsbwxrc.html

F. 文件与目录
来源：http://hz.cheryme.top/gtdkljfnow.html

================================================================================
来源：http://hz.316326.xyz/gtjxiruqrf.html

[F01] 读取整个文件
来源：http://hz.shanyushiyangkeji.top/gtvxuipvks.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenzaomai.com/gtaddneopv.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhongyouzk.top/gtmllwsbaf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.wangdashe.top/gtqbabjtxv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.redwolf501.top/gtfxwleqas.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtijildoeq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhixingplan.top/gtixzgrzhk.html

Ruby: File.read("a.txt")
来源：http://hz.nanxinkj.top/gtksmwvhrj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cheryme.top/gtxycxpppg.html

[F02] 逐行读取文件
来源：http://hz.bjfxy.top/gtptekkbia.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.snrcjt.cn/gtndisbkbn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yanxiufei.cn/gtmolbqbpv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtxczzpeec.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgufenzy.top/gtxufjcqpn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xinyue.icu/gtzziyeyzk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sysykeji.top/gtsfhwywog.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.fzhhl.top/gtoxtssagk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinqigufen.top/gtmolmxqwa.html

[F03] 写入文件（覆盖）
来源：http://hz.yueranfly.top/gtymvepqiv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jlsjyb.cn/gtjnboqqwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.nanxuanxn.top/gtazsivlmz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtybdlubdl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cashguo.top/gtrwwxhvao.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jqgfzy.top/gtuzusfwdu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.fzhhl.top/gtrxakaipl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.smart0.xyz/gtttwftenk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.0kj1m.cn/gtxrhljuuz.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gtcnmpjgdk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xuetiantiany.cn/gtpqydsozy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hysaishi.cn/gtjnqygolp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangkeji.top/gtubirrdiw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtvrehugku.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.chenzaomai.com/gtyzqaeauw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.fengsongda.top/gtgfkzovxn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.pengpengdd.cyou/gtsahhqbeb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.tanke756.top/gtiyransgi.html


<!-- 参考信息 -->