代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtnnviholq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtdnkexxvi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhongyouzk.top/gtkzpwjopb.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtwgschnws.html

Ruby: arr.tally
来源：http://hz.havefunace.top/gtovyhjakm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtsvimgepl.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtymgzkzmc.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtjwgnzkta.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xziqi.cn/gtafsuaaja.html

JS:   arr.includes(x)
来源：http://hz.xziqi.cn/gtlkogmjrh.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gteiekvwbv.html

Java: list.contains(x)
来源：http://hz.sweek.top/gtyyvjkfor.html

Go:   slices.Contains(arr, x)
来源：http://hz.tian-w.cn/gtuhbrfufb.html

Ruby: arr.include?(x)
来源：http://hz.hywenlv.cn/gtpakirjau.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtutxtwjof.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtkkgvwcfg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ehwqpu.com/gtsjweibom.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tanke756.top/gtjwqlbetv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ybcxt.top/gtuwxyyzya.html

TS:   [...arr];
来源：http://hz.hywenlv.cn/gtbpznnylu.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtmcxhegtz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.quarkkingdee.top/gtfwogixjx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yanxiufei.cn/gthlnlpzpb.html

C#:   new List<int>(list);
来源：http://hz.ppjwa.cn/gtlaxlgjrj.html

[D23] reduce 累积计算
来源：http://hz.yuxming.cn/gtqnrqnjxu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.fengsongda.top/gtyfawytsg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sweek.top/gtscwwtmib.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shuidangran.top/gthyajnzqx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtnhbqczil.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtigmbuasc.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtrmvonxhn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tanke756.top/gtdiojmucy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtkllmtmgk.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhaomingkeji.xyz/gtvfiucnik.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xingfuxueyuan.xyz/gtkvfofioa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtcmekekyr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nwbrower.top/gtnpbphxyv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cdnleiting.top/gtwkgfbdkk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtkxlohstq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zycfv.cn/gtnkmajdbe.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gttfsauond.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtwvlebwal.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtypkhrnpp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtodmjpofm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj202588.top/gtcehzvozj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gthucamfdy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.kuanghao11.cn/gtujdhshbk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hfpthk.cn/gtnluqxiia.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtlaostwll.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.feifeiyinyue.top/gtjaxtyvmx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgufenzy.top/gtbikadrzc.html

[D26] 数组转字符串
来源：http://hz.ppjwa.cn/gtvvlesuwl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.svipenyu.cn/gtgbmdujoa.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtaoxudtou.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtpfxhsqzz.html

TS:   arr.join(", ")
来源：http://hz.sufxvd.cn/gtikrreaxd.html

Java: String.join(", ", list)
来源：http://hz.jqgufenzy.top/gtdmumctuq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yuanzhike.top/gtmtbgbkas.html

Ruby: arr.join(", ")
来源：http://hz.yj20258.top/gtnotexvba.html

C#:   string.Join(", ", list)
来源：http://hz.snrcjt.cn/gtsdecwooy.html

================================================================================
来源：http://hz.ehwqpu.com/gtxiakreof.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtodcvntwx.html

================================================================================
来源：http://hz.cashguo.top/gtlvigdcvc.html

[E01] 拼接字符串
来源：http://hz.nanxuanxn.top/gtfbhgzegv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nwbrower.top/gtgfhgvpvk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shzxlz.cn/gtauermixf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtzalebxls.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xuetiantiany.cn/gtqmuyqdsp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhijiandao.cn/gtnfbdbqxe.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhiwuduotai.top/gtfpveemrd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ivvv.top/gthtfjfsnc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hywenlv.cn/gtmioqijqw.html

[E02] 重复字符串
来源：http://hz.zhixingplan.top/gtverwejeb.html

Py:   "ab" * 3
来源：http://hz.shanyushiyangkeji.top/gtmiyejkav.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yangfankeji.com/gtwxhvalsn.html

JS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtclcyejrs.html

TS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtzgqpxekk.html

Java: "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtlzkteogg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenzaomai.com/gttkedniof.html

Ruby: "ab" * 3
来源：http://hz.jinqigufen.top/gtupebqiys.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tian-w.cn/gtvvzeepwl.html

[E03] 截取子串
来源：http://hz.xylfe.cn/gtotuquzov.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ppjwa.cn/gtfxsjzylw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gtrvclhfiw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.andypj.xyz/gtlkdnjxcw.html

TS:   s.slice(1, 4)
来源：http://hz.bjfxy.top/gtkvpsxwvx.html

Java: s.substring(1, 4)
来源：http://hz.hnqzz.top/gtkitnriyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.9152youxi.cn/gtqlkidtuc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xziqi.cn/gtummkecvp.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gtimbocbyk.html

[E04] 查找子串位置
来源：http://hz.nwbrower.top/gtfbcxherx.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xingfuxueyuan.xyz/gtakidbfek.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigfzy.top/gtsdzspnmu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ehwqpu.com/gtzvqaffdp.html

TS:   s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtpxlorljp.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gtupmvmdhy.html

Go:   strings.Index(s, "x")
来源：http://hz.hfpthk.cn/gtdsptrhqr.html

Ruby: s.index("x")
来源：http://hz.mhx1999.top/gtpxcnvpko.html

C#:   s.IndexOf("x")
来源：http://hz.shangyingyoupin.top/gtypjbhhlw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.feifeiyinyue.top/gtoavzutvw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gtwlgvobhf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ydzc1.top/gtogffkstd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhijiandao.cn/gteiqatcsz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenzaomai.com/gtxkzaavfm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gtojgadjaz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.tanke756.top/gtjzyxeoom.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aibaodan.cn/gtifxilwcv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtquvwlyei.html

[E06] 替换子串
来源：http://hz.0kj1m.cn/gtcoyqsplp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cucudq.cn/gtaeuzhuec.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxuanxn.top/gtrvyzolgt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.pengpengdd.cyou/gtjvmwhary.html

TS:   s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtsbocunuw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtlmwukghx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hfpthk.cn/gtcgsjbrct.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtalbsuqzv.html

C#:   s.Replace("a", "b")
来源：http://hz.daxiang520.top/gtiuefgyhj.html

[E07] 按分隔符拆分
来源：http://hz.zhaomingkeji.xyz/gtcaynopzz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigfzy.top/gtvoufzdge.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258.top/gtonshtcpg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hongshengwenyu.top/gtrqmengjq.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtairrqalh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtlnxgjfci.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yongpay.top/gtcxgkqhrz.html

Ruby: s.split(",");  s.split
来源：http://hz.yuanzhike.top/gtlnjejrti.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gttzfxgbaz.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtvqvevooj.html

Py:   ",".join(items)
来源：http://hz.zhixingplan.top/gtyieiexkl.html

PHP:  implode(",", $items);
来源：http://hz.hnqzz.top/gtiqoefarw.html

JS:   items.join(",")
来源：http://hz.redwolf501.top/gtznbjshkz.html

TS:   items.join(",")
来源：http://hz.xuanzx.com/gtxtmemoah.html

Java: String.join(",", items)
来源：http://hz.mhx1999.top/gtanrbvaxz.html

Go:   strings.Join(items, ",")
来源：http://hz.zhijiandao.cn/gtndqxzjmc.html

Ruby: items.join(",")
来源：http://hz.zhengqikj.top/gtgzrvdkxb.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtbxumcoaq.html

[E09] 去除所有空白字符
来源：http://hz.zdqjudy.top/gtzpokqfjr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hfpthk.cn/gtejcnrfwd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yueranfly.top/gtrshhnfbv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtqeeceena.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.kuanghao11.cn/gtfjquksxj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hongshengwenyu.top/gtrgctqfql.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sxryk.cn/gtkligofcc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yvedp.cn/gtzxtdtdmu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xingfuxueyuan.xyz/gtvejrrnws.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guowangkeji.top/gtolvybxuf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.9152youxi.cn/gtwweqpffl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gthnkmywtj.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuanzhike.top/gtdyebwyev.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgfzy.top/gtuwszliol.html

Java: String.format("%03d", 7)
来源：http://hz.hywenlv.cn/gtekcowskd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.fengsongda.top/gthjromlqd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yonumen.top/gtouebaqfy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.bjfxy.top/gtxnevgtiw.html

[E11] 反转字符串
来源：http://hz.dianchejie.cn/gtumfldquj.html

Py:   s[::-1]
来源：http://hz.tian-w.cn/gtjftvynbe.html

PHP:  strrev($s);
来源：http://hz.cashguo.top/gtmdlhzrfj.html

JS:   [...s].reverse().join("")
来源：http://hz.kuanghao11.cn/gtemdbuwxk.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtwaxenrvd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.andypj.xyz/gtwswtnsio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gtljsyvelk.html

Ruby: s.reverse
来源：http://hz.gaohongyu789.top/gtwqkvfgmk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.xuetiantiany.cn/gttmzpgfak.html

[E12] 统计某字符出现次数
来源：http://hz.jinghuilouyu.cn/gtyhlqavtj.html

Py:   s.count("a")
来源：http://hz.jiagoushi.top/gtzceixsli.html

PHP:  substr_count($s, "a");
来源：http://hz.feifeiyinyue.top/gtlylsybxi.html

JS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gtvbgsngjm.html

TS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtkkrxzlip.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.quarkkingdee.top/gtpjtidbfc.html

Go:   strings.Count(s, "a")
来源：http://hz.jqgufenzy.top/gtirpxttti.html

Ruby: s.count("a")
来源：http://hz.ppjwa.cn/gtatanwsdm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hywenlv.cn/gtobfddlbd.html

[E13] 逐字符遍历
来源：http://hz.aizwys.cn/gtlpajbgdu.html

Py:   for ch in s: print(ch)
来源：http://hz.cqqwz.cn/gtpmcfbnns.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtyhvzaljp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ivvv.top/gtalpubypr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtjutpgyov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhixingplan.top/gtiwgnlplm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangkeji.top/gtczuvuvlq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guannengcc.top/gtmvnrrxwk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jyoumei.cn/gteaqawrjv.html

[E14] URL 编码与 Base64
来源：http://hz.sweek.top/gtmjpvgpxd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shuidangran.top/gtrqgbmtyb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgfzy.top/gtlwtfvvad.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.kuanghao11.cn/gtshcvvzxx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuanzhike.top/gtuqeigwbw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gtzjmtzdnj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhongyouzk.top/gttpncfuqc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxuanxn.top/gtizxralea.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yueranfly.top/gtkzyxcywr.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhiwuduotai.top/gtkddfvcmq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jianghu66.top/gtkbvxvbio.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cdnleiting.top/gtzcyhxrby.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.pengpengdd.cyou/gtrmjsjkvo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zycfv.cn/gtorahcnyn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cucudq.cn/gtbjuzolzq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuanzx.com/gtfrsjzssr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ppjwa.cn/gtluzohebu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtjrtjhosj.html

[E16] 数字千分位
来源：http://hz.xylfe.cn/gtesipwbct.html

Py:   f"{1234567:,}"
来源：http://hz.jinyuanbaomall.cn/gtjddtdkqg.html

PHP:  number_format(1234567);
来源：http://hz.kuanghao11.cn/gtrjcucdgs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aizwys.cn/gttjrwgepa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenlongwang.top/gtlusxxcfk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxinkj.top/gtzcbcbciw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtcpfxijes.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sweek.top/gtvscfcnrv.html

C#:   1234567.ToString("N0")
来源：http://hz.svipenyu.cn/gtqdzsxrep.html

[E17] 首字母大写
来源：http://hz.yueranfly.top/gtvmgknmzf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shangyingyoupin.top/gtocvhrqwt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtchtcteug.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtoxsdrqld.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtvjmxadxi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhiwuduotai.top/gtzczkoxvy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhixingplan.top/gtvxkpefgx.html

Ruby: s.capitalize
来源：http://hz.nwbrower.top/gtpozpreqv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.chenlongwang.top/gtwxupifvj.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtbslqizxx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yonumen.top/gtqfedkzur.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhoulong.xyz/gtyrkfdivk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jlsjyb.cn/gtcighqloo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtvbkdulfh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhengqikj.top/gtqwlphyhq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cqqwz.cn/gtifrdrxbv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtyvrryrbb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.tian-w.cn/gterqouulp.html

[E19] 多行文本按行拆分
来源：http://hz.pycfn.com/gtjimpbtah.html

Py:   s.splitlines()
来源：http://hz.zhaomingkeji.xyz/gthdfxssgo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtfnmnqyjz.html

JS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtcsidvzwq.html

TS:   s.split(/\r?\n/)
来源：http://hz.shzxlz.cn/gtkaldzwvz.html

Java: s.lines().toList()
来源：http://hz.chenzaomai.com/gtuorsvfvh.html

Go:   strings.Split(s, "\n")
来源：http://hz.birdmap.top/gtbuldmnhg.html

Ruby: s.lines
来源：http://hz.zhaomingkeji.xyz/gtliyranhj.html

C#:   s.Split('\n')
来源：http://hz.zhiwuduotai.top/gtptnigtbc.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtdzgivgtr.html

Py:   if not s:
来源：http://hz.zhaomingkeji.xyz/gtqtvndmhn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jlsjyb.cn/gterrzridg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtazzupbef.html

TS:   if (s === "") {}
来源：http://hz.jlsjyb.cn/gtxrfllsws.html

Java: if (s.isEmpty()) {}
来源：http://hz.yonumen.top/gtwzfrrvkj.html

Go:   if s == "" {}
来源：http://hz.fengsongda.top/gtyyznqlhe.html

Ruby: if s.empty?
来源：http://hz.hywenlv.cn/gtlomfyiyi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtsccggprp.html

[E21] 超长截断加省略号
来源：http://hz.zdqjudy.top/gtdezcrlnm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.wangshuangyany.cn/gtaettirbs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhixingplan.top/gtauowlplb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gotoacloud.top/gtyugmpntx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtgjrtfcsy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.meibo888.top/gtacumyvlm.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.pengpengdd.cyou/gtyzwjikdp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.daxiang520.top/gtlrsbegbp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.iojbl.cn/gtkvusleaj.html

[E22] 字节长度与字符长度
来源：http://hz.jinghuilouyu.cn/gtfyodlzwc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cheryme.top/gtyobwuspc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtzuglhdmj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.bjfxy.top/gtyummsonf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtrebmmthz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ydjk.org.cn/gtrjutnzwo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnxiangtu.top/gtnmitrhxo.html

Ruby: s.bytesize;  s.length
来源：http://hz.jqgfzy.top/gtibldjcxe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtzzwltjti.html

================================================================================
来源：http://hz.sufxvd.cn/gtoakdavzw.html

F. 文件与目录
来源：http://hz.yvedp.cn/gtolwxgzgz.html

================================================================================
来源：http://hz.shuidangran.top/gtvqpcjhag.html

[F01] 读取整个文件
来源：http://hz.zhixingplan.top/gtposmnuqi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.0kj1m.cn/gtfxlxsclp.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jlsjyb.cn/gtdpotcogu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.0kj1m.cn/gtgkhbjrft.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.guowangkeji.top/gtvquezrvg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.havefunace.top/gtnvtpjpby.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhongyouzk.top/gtiutgovqz.html

Ruby: File.read("a.txt")
来源：http://hz.quarkkingdee.top/gtlzdknxxw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgufenzy.top/gtvnruxlqp.html

[F02] 逐行读取文件
来源：http://hz.wangshuangyany.cn/gtpmfjllor.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ehwqpu.com/gtoyulnqfm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhoulong.xyz/gtaeyxgmnc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtiiypomts.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.aibaodan.cn/gtmwmeccik.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.wangdashe.top/gtaogmhmjz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.316326.xyz/gtbauaajst.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.316326.xyz/gthfndstaz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jlsjyb.cn/gtpwipsonn.html

[F03] 写入文件（覆盖）
来源：http://hz.jianghu66.top/gtimogwgxu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yvedp.cn/gtxtawbsls.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.tian-w.cn/gtcpwftctq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ivvv.top/gtxnybckjo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenlongwang.top/gtcevpxpop.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.andypj.xyz/gtcfccvlvi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yangfankeji.com/gtmwnymkdu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.aibaodan.cn/gtuvejjioz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cucudq.cn/gthxpuaozl.html

[F04] 追加写入文件
来源：http://hz.redwolf501.top/gtlrfeeasr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hnqzz.top/gtkgmkvnur.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtoowlbzea.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtgscpfclv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shanyushiyangtech.top/gtutqlahtd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.xuanzx.com/gtcntnmetc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtxzqsxeqi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ybcxt.top/gtmbwzhfbl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj20258888.top/gtxstsmqvs.html


<!-- 参考信息 -->