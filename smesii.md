代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtilijwhir.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtpusloxlw.html

Go:   // 手写 map[string][]T
来源：http://hz.chenlongwang.top/gtfaawskjp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhijiandao.cn/gthfpfrhot.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtrbkudodn.html

[D20] 统计每个元素出现次数
来源：http://hz.guannengcc.top/gtvaawnznt.html

Py:   Counter(arr)
来源：http://hz.gaohongyu789.top/gtiyuwowit.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtqiciewsp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtppzdgryo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtqeiekqpy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.bjfxy.top/gtbndlmyqh.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtjbmpsfyb.html

Ruby: arr.tally
来源：http://hz.feifeiyinyue.top/gthfmkgjom.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtzbvrfafh.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtwbvdvsxr.html

Py:   x in arr
来源：http://hz.chenlongwang.top/gtreetjnvj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtljsjsioy.html

JS:   arr.includes(x)
来源：http://hz.316326.xyz/gtfipyvrad.html

TS:   arr.includes(x)
来源：http://hz.316326.xyz/gtucxtthaw.html

Java: list.contains(x)
来源：http://hz.wangshuangyany.cn/gtzeqxwwje.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtknlraksd.html

Ruby: arr.include?(x)
来源：http://hz.jyoumei.cn/gtfsjrnsue.html

C#:   list.Contains(x)
来源：http://hz.fzhhl.top/gtzhjwylkf.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aibaodan.cn/gtnoxqpxgr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtpniqrvro.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtpacahlgo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangshuangyany.cn/gtquvyajbw.html

TS:   [...arr];
来源：http://hz.0kj1m.cn/gtvbszbqsg.html

Java: new ArrayList<>(list);
来源：http://hz.gaohongyu789.top/gttisczpaq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cheryme.top/gtadfzhxwa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhijiandao.cn/gtzrjlmifm.html

C#:   new List<int>(list);
来源：http://hz.hnqzz.top/gtkxvfcumy.html

[D23] reduce 累积计算
来源：http://hz.hongshengwenyu.top/gtuutbletd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sysykeji.top/gtpuntxatm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhijiandao.cn/gtrbhovqam.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xingfuxueyuan.xyz/gtytkytsfs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtmuomfmyz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.vqdsnc.cn/gtkwlibxwr.html

Go:   // 手写循环
来源：http://hz.yanxiufei.cn/gtrvxuamvk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gtlinnofbx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daxiang520.top/gtwvhirexi.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtgwxgzghv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gtgmgdnnss.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jqgfzy.top/gtgotvgliq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.meibo888.top/gteqazkrqp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.meibo888.top/gtuztbysdc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.kuanghao11.cn/gtwzqiuyyu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtoattqovy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtmhlqvvvj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cucudq.cn/gtlphjugpo.html

[D25] Set 集合去重与交并差
来源：http://hz.cqqwz.cn/gtsvftchgg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.redwolf501.top/gtfljmdktq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtuxszrxmi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhijiandao.cn/gtdpiljujf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zdqjudy.top/gtqcgadyfs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tianlin.xyz/gtrstnnjca.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gtepcmadjc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258.top/gtqwriowgv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yonumen.top/gtvoczpvcv.html

[D26] 数组转字符串
来源：http://hz.zhoulong.xyz/gtnvtgomrl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhongyouzk.top/gtvvyidntw.html

PHP:  implode(", ", $arr);
来源：http://hz.gzhubu.top/gtupqpfjkp.html

JS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtzqikeznm.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtlwsxtjkg.html

Java: String.join(", ", list)
来源：http://hz.jinqigfzy.top/gtximbllpz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.mhx1999.top/gtcsmqcogc.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtsjbveixp.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258.top/gthtpowsjf.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlefykzcf.html

E. 字符串处理
来源：http://hz.shzxlz.cn/gtkogmzjjx.html

================================================================================
来源：http://hz.yuxming.cn/gtjccureij.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtxenulcwv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xinyue.icu/gtiphyvtbx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinqigufen.top/gtqxepyypc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtjluvzvyx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtebdwcoqh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gtaapxzyxc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.iojbl.cn/gtbblacnzz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtwlixpgul.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.snrcjt.cn/gtlsfrqitn.html

[E02] 重复字符串
来源：http://hz.c1oappe.top/gtiynwvxth.html

Py:   "ab" * 3
来源：http://hz.shangyingyoupin.top/gthqtutuyl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtkoqvhwrh.html

JS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtbnojzetd.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtlwxeoano.html

Java: "ab".repeat(3)
来源：http://hz.xziqi.cn/gtweljlxjp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sweek.top/gtglaqyjrd.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtxqoqxnmm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtbbgiqkpy.html

[E03] 截取子串
来源：http://hz.yonumen.top/gtfohpetew.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cheryme.top/gtahzstrpo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yvedp.cn/gtznhxpbuv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtcsmhhgsu.html

TS:   s.slice(1, 4)
来源：http://hz.daria6918.cn/gtirjwovye.html

Java: s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtvbyiizfo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yvedp.cn/gtzurmhvzn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.smart0.xyz/gtjfhespso.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtwnnktyyh.html

[E04] 查找子串位置
来源：http://hz.shanyushiyangkeji.top/gtyrduzfsg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zdqjudy.top/gtbotwdzlv.html

PHP:  strpos($s, "x");
来源：http://hz.zhiwuduotai.top/gtruwylqnx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtnnecxcsf.html

TS:   s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtmdwnaiys.html

Java: s.indexOf("x")
来源：http://hz.gzhubu.top/gtukbouvkg.html

Go:   strings.Index(s, "x")
来源：http://hz.hysaishi.cn/gtkynduslk.html

Ruby: s.index("x")
来源：http://hz.jiagoushi.top/gtdggqbyxc.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gtsxdfhvra.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gtlrlilcoy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj202588.top/gtzdwtpkpz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jiagoushi.top/gtrkbfooij.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gthqrkqhqc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.daria6918.cn/gtqixqpojc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gtjaitoumz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtunovxicn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fengsongda.top/gtsvquvrva.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xylfe.cn/gtubrgtztn.html

[E06] 替换子串
来源：http://hz.zhaomingkeji.xyz/gtgxjbgwnu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.316326.xyz/gtgnmoxfwr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtchpcanbj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtqtjqcpdm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtsbonkqgb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtlvikszpa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tianlin.xyz/gthaozqyhd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yvedp.cn/gtocnspeor.html

C#:   s.Replace("a", "b")
来源：http://hz.wangshuangyany.cn/gtiuawmydc.html

[E07] 按分隔符拆分
来源：http://hz.316326.xyz/gtdahjgxam.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.gaohongyu789.top/gtczzekyfn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ybcxt.top/gthofzdxxh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ybcxt.top/gttysgdgub.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtwrljddex.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hnxiangtu.top/gthoaahvxa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fengsongda.top/gtfntugufi.html

Ruby: s.split(",");  s.split
来源：http://hz.gogol.net.cn/gtlgstjnih.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sysykeji.top/gtqbcrprxk.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtasukgrtq.html

Py:   ",".join(items)
来源：http://hz.shanyushiyangtech.top/gtujpptuws.html

PHP:  implode(",", $items);
来源：http://hz.xingfuxueyuan.xyz/gtdfnuwulx.html

JS:   items.join(",")
来源：http://hz.cqqwz.cn/gtehetxfat.html

TS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtbbcfrfnq.html

Java: String.join(",", items)
来源：http://hz.cdnleiting.top/gtjmypnxgw.html

Go:   strings.Join(items, ",")
来源：http://hz.0kj1m.cn/gtjwkrhchc.html

Ruby: items.join(",")
来源：http://hz.ydjk.org.cn/gtekqzstcb.html

C#:   string.Join(",", items)
来源：http://hz.sweek.top/gtgbxasiwo.html

[E09] 去除所有空白字符
来源：http://hz.yonumen.top/gtfkdlxpia.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.havefunace.top/gtdgsthbmz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shangyingyoupin.top/gtvqibsfoj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gtiyrawqaj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtlaxxsrgv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtvashigce.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yuxming.cn/gtehxmqkth.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xuetiantiany.cn/gtcvpbuhkm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cqqwz.cn/gtjaiobxau.html

[E10] 左侧补零 / 定长填充
来源：http://hz.smart0.xyz/gtxkvljven.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yvedp.cn/gtndvjoovg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aizwys.cn/gthmmzkckk.html

JS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtmaytzyht.html

TS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtfpmagmzr.html

Java: String.format("%03d", 7)
来源：http://hz.52xcode.cn/gtofrclpyz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.wangdashe.top/gtiurdlnyd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtfklonblv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zycfv.cn/gtmcjharxq.html

[E11] 反转字符串
来源：http://hz.hammf.cn/gtmrwwbgjs.html

Py:   s[::-1]
来源：http://hz.iojbl.cn/gttnbnxgvx.html

PHP:  strrev($s);
来源：http://hz.gaohongyu789.top/gthgjtplcl.html

JS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtnunvvtje.html

TS:   [...s].reverse().join("")
来源：http://hz.yueranfly.top/gtwmamjbgd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtxajiieju.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.daxiang520.top/gtpmgvczbg.html

Ruby: s.reverse
来源：http://hz.316326.xyz/gtqjjizuht.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.wangdashe.top/gtxirgbvtd.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigufen.top/gtuxeqiele.html

Py:   s.count("a")
来源：http://hz.vqdsnc.cn/gtxqqjfjtk.html

PHP:  substr_count($s, "a");
来源：http://hz.yuxming.cn/gtyddebdup.html

JS:   s.split("a").length - 1
来源：http://hz.ydzc1.top/gtmkihhoqr.html

TS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtnkswmxjg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtubfrmlxg.html

Go:   strings.Count(s, "a")
来源：http://hz.ywan-chungtsiang.top/gtsdptlueg.html

Ruby: s.count("a")
来源：http://hz.meibo888.top/gtkqxottia.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtidwweouv.html

[E13] 逐字符遍历
来源：http://hz.ehwqpu.com/gteprchffk.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtxnpcnlfm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.birdmap.top/gtqehwuonl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtcqhduglh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtpoymurap.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xinyue.icu/gttftbhaov.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtyljpxold.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.quarkkingdee.top/gtdxysimvm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cheryme.top/gtxaqpjtan.html

[E14] URL 编码与 Base64
来源：http://hz.pengpengdd.cyou/gtxznwyvez.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cucudq.cn/gtnyqcxarl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gthvswyuft.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj20258888.top/gtofnqcnbd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.svipenyu.cn/gtdujpcpho.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shanyushiyangtech.top/gtsehafasn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinqigufen.top/gtzupqqrgn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sufxvd.cn/gtspqllwuk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gaohongyu789.top/gtmenbubqq.html

[E15] HTML 转义 / 反转义
来源：http://hz.yueranfly.top/gtrmlbptrx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.9152youxi.cn/gtanjfvfwk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cdnleiting.top/gtapdjwnsx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zhongyouzk.top/gtqbtkhuwu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gotoacloud.top/gtyiayjijy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ywan-chungtsiang.top/gtxdsjovbz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhongyouzk.top/gtfwzzbpfn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtwkxwdyye.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.quarkkingdee.top/gtcrmsxzdz.html

[E16] 数字千分位
来源：http://hz.pycfn.com/gtkuyctabs.html

Py:   f"{1234567:,}"
来源：http://hz.aizwys.cn/gthzadirle.html

PHP:  number_format(1234567);
来源：http://hz.hysaishi.cn/gtckkgznwt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.0kj1m.cn/gtqtiatlwm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtgprppqiz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jqgufenzy.top/gtrnyulzwn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.havefunace.top/gtundyglpk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gaohongyu789.top/gtsifjciro.html

C#:   1234567.ToString("N0")
来源：http://hz.ybcxt.top/gtmjchnoha.html

[E17] 首字母大写
来源：http://hz.yuxming.cn/gtmnucizbi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenjidiqi.icu/gtzvyhtonq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.0kj1m.cn/gtvgvljnir.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yongpay.top/gtrhquodkw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.52xcode.cn/gtoiafiasf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtyxioencq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xziqi.cn/gtqhotlogu.html

Ruby: s.capitalize
来源：http://hz.quarkkingdee.top/gtktxldxrp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jlsjyb.cn/gtbhhhkxmq.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtvhnuaxyx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ybcxt.top/gtdamzfkuo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hywenlv.cn/gtqkkzhylg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtsummneek.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gttfwxtusm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhengqikj.top/gtjohtaeaf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuanzx.com/gtyrmyfzxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.tian-w.cn/gtiegrkryq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnqzz.top/gtthzqzrxb.html

[E19] 多行文本按行拆分
来源：http://hz.mhx1999.top/gtpiovuwyq.html

Py:   s.splitlines()
来源：http://hz.nanxuanxn.top/gtprerryym.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jiagoushi.top/gtojlgzeqf.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtxdzrhzzj.html

TS:   s.split(/\r?\n/)
来源：http://hz.wangdashe.top/gtstvbbgqd.html

Java: s.lines().toList()
来源：http://hz.zycfv.cn/gtrxdsdpvn.html

Go:   strings.Split(s, "\n")
来源：http://hz.hammf.cn/gtayudndjz.html

Ruby: s.lines
来源：http://hz.dianchejie.cn/gtepsputcy.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gtacainfvp.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtnbcuhyqx.html

Py:   if not s:
来源：http://hz.zhiwuduotai.top/gtaxpqcuzq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigfzy.top/gtatcuzcso.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.chenjidiqi.icu/gtinqgqtzf.html

TS:   if (s === "") {}
来源：http://hz.jianghu66.top/gtmffiyehk.html

Java: if (s.isEmpty()) {}
来源：http://hz.feifeiyinyue.top/gtbtadrgdz.html

Go:   if s == "" {}
来源：http://hz.yj202588.top/gtapqgynlo.html

Ruby: if s.empty?
来源：http://hz.yvedp.cn/gtdytkzdht.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.haohaochexian.top/gtcctfztmf.html

[E21] 超长截断加省略号
来源：http://hz.ydzc1.top/gtizeeyuox.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtphdfhlin.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.iojbl.cn/gtqghiaksq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtqbjtbplc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtoqvutowm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtmwhlumvh.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.cdnleiting.top/gtmfrdrfeb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yj20258888.top/gtitsegpya.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.quarkkingdee.top/gtkfwafhwe.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtspwurgyx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yonumen.top/gtgnvpvnit.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtviqigwnu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtifpirimh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtjfdawmgy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gtnpfpztnr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.redwolf501.top/gtjfgjjvrw.html

Ruby: s.bytesize;  s.length
来源：http://hz.bjfxy.top/gthnusssta.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gttexukcos.html

================================================================================
来源：http://hz.jyoumei.cn/gtrzjoasso.html

F. 文件与目录
来源：http://hz.redwolf501.top/gtjaliyetw.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtoakxwiti.html

[F01] 读取整个文件
来源：http://hz.0kj1m.cn/gtitjebkhs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtteirfvcl.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gotoacloud.top/gtvtwfncfs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.52xcode.cn/gtupgtqcwf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sweek.top/gtytftrbip.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtnufaxozv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.shanyushiyangkeji.top/gttpzxrhgs.html

Ruby: File.read("a.txt")
来源：http://hz.shanyushiyangtech.top/gtmiksgafc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtqycgepwz.html

[F02] 逐行读取文件
来源：http://hz.sweek.top/gtwkmgiuqm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgufenzy.top/gtousdbrxc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.fengsongda.top/gthtkjtrun.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cqqwz.cn/gtwdoxnptr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hysaishi.cn/gtaopqajjc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtzajdcizh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tanke756.top/gtonktbwyh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhiwuduotai.top/gtovebbgdw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.birdmap.top/gtfxxnhiyr.html

[F03] 写入文件（覆盖）
来源：http://hz.haohaochexian.top/gtbcecudrm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydzc1.top/gtrlxjuvpt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jqgufenzy.top/gtjxjnwofs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.wangshuangyany.cn/gtlgpxhnky.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtnzqtnggr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.xylfe.cn/gtqypeuwde.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinyuanbaomall.cn/gtgtardnkv.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhiwuduotai.top/gtccdsmxzv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ydzc1.top/gtjurttedd.html

[F04] 追加写入文件
来源：http://hz.gotoacloud.top/gthcgbvltd.html


<!-- 参考信息 -->