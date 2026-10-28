代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yanxiufei.cn/gtosdegjxn.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtdwkcvxls.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtvewrakra.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtpbhlvxzp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.9152youxi.cn/gtiebcruex.html

PHP:  array_merge(...$nested);
来源：http://hz.tian-w.cn/gtqkqeseai.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gttczzqkgf.html

TS:   nested.flat();
来源：http://hz.sweek.top/gtoizygfye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cheryme.top/gtwlsxavjb.html

Go:   // 手写双层循环
来源：http://hz.zdqjudy.top/gtdjzovuvi.html

Ruby: nested.flatten
来源：http://hz.zhixingplan.top/gtgrpsejub.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jyoumei.cn/gtupwkcugp.html

[D19] 按字段分组
来源：http://hz.fzhhl.top/gtoowuagfg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtpydluhxu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cucudq.cn/gtblmfhbel.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtzpfpdybz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtfcrbeebt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigfzy.top/gtujhewakf.html

Go:   // 手写 map[string][]T
来源：http://hz.aibaodan.cn/gtusqcmnet.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtakdyudql.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinyuanbaomall.cn/gtasiyzyga.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258.top/gtwjormjkg.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtsmkgkmlf.html

PHP:  array_count_values($arr);
来源：http://hz.cdnleiting.top/gtctrtoirp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtrosbzfjj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtziwkufmv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtbgjkoczw.html

Go:   // 手写 map[T]int
来源：http://hz.zhongyouzk.top/gtslifwacz.html

Ruby: arr.tally
来源：http://hz.shzxlz.cn/gtlendixfv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.smart0.xyz/gthbnasqbk.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtxewjskol.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtoqsjkhba.html

PHP:  in_array($x, $arr, true);
来源：http://hz.haohaochexian.top/gtmsdbwhrx.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtjfyuehxs.html

TS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtbdbjsere.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtwxibslnz.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gtzlwnrzez.html

Ruby: arr.include?(x)
来源：http://hz.52xcode.cn/gttckutbzi.html

C#:   list.Contains(x)
来源：http://hz.meibo888.top/gtfifvzest.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj202588.top/gtngflriiw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pengpengdd.cyou/gtdjdhztpe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cheryme.top/gtkzrkroyu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gtavuixqri.html

TS:   [...arr];
来源：http://hz.zhengqikj.top/gtbjrcaork.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtlgiazusd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yongpay.top/gthohhjrar.html

Ruby: arr.dup;  arr.clone
来源：http://hz.0kj1m.cn/gtyswpfhdy.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtbbvowmei.html

[D23] reduce 累积计算
来源：http://hz.havefunace.top/gtltnkispp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtfkgvpulg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.52xcode.cn/gtqfzxwsxv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gtbwrwqbda.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhixingplan.top/gtrtsbbbjp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yuanzhike.top/gtagnecxri.html

Go:   // 手写循环
来源：http://hz.xuanzx.com/gtoafkgcse.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.0kj1m.cn/gtdemxtxaz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zycfv.cn/gtdbpdyjpe.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuetiantiany.cn/gtbycasiqo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gtlqrkglsw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.kuanghao11.cn/gtfgebuvpz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj202588.top/gtznfufyqb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtgujzxqxe.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yvedp.cn/gtwfuxyoby.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinqigfzy.top/gtqaykxzxa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cheryme.top/gtgwhvhivh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.snrcjt.cn/gtqcjhivee.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtrejdwjbk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.birdmap.top/gtfcqglskj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtsavwefhr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhijiandao.cn/gtyactcfop.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.meibo888.top/gthxdfvacc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daria6918.cn/gtbkpliter.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sufxvd.cn/gtdrunwrcj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtivmqcaec.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtocicgkhd.html

[D26] 数组转字符串
来源：http://hz.jinqigfzy.top/gtdxvwjnls.html

Py:   ", ".join(map(str, arr))
来源：http://hz.iojbl.cn/gtmqdkpnbr.html

PHP:  implode(", ", $arr);
来源：http://hz.nwbrower.top/gtfibefaem.html

JS:   arr.join(", ")
来源：http://hz.yanxiufei.cn/gtofmhzzom.html

TS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gttvlmfusn.html

Java: String.join(", ", list)
来源：http://hz.nanxuanxn.top/gtgrbucrte.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jyoumei.cn/gtyyjtgqjm.html

Ruby: arr.join(", ")
来源：http://hz.hywenlv.cn/gtdmywsepb.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtguveuugf.html

================================================================================
来源：http://hz.gotoacloud.top/gtfhqbrdhj.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtcdtnnezz.html

================================================================================
来源：http://hz.yuxming.cn/gtcheggbmk.html

[E01] 拼接字符串
来源：http://hz.andypj.xyz/gtdrpfvgqv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hnqzz.top/gttiejxkmf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zdqjudy.top/gtgagjmkjd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtlqxxdkye.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gttiaalbug.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.iojbl.cn/gtkabxtara.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sweek.top/gtnexstoeu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gtxctbgtzl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtgceqzgab.html

[E02] 重复字符串
来源：http://hz.snrcjt.cn/gtcdtnzjfy.html

Py:   "ab" * 3
来源：http://hz.ydjk.org.cn/gtmmehbfqe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.quarkkingdee.top/gtpneophij.html

JS:   "ab".repeat(3)
来源：http://hz.zycfv.cn/gtimtvldsx.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtvdsigmtv.html

Java: "ab".repeat(3)
来源：http://hz.nwbrower.top/gtcbfylnvo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shangyingyoupin.top/gtpgraqpws.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtbliczrkw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yueranfly.top/gtiayfolxr.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gthcngwqlq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zycfv.cn/gtulljasai.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ehwqpu.com/gttecbxmrb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ehwqpu.com/gtpthnaqgc.html

TS:   s.slice(1, 4)
来源：http://hz.xuetiantiany.cn/gtbadezqaj.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtnymsquyr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hysaishi.cn/gtrvgbjism.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xziqi.cn/gtjdpqsdbd.html

C#:   s.Substring(1, 3)
来源：http://hz.jiagoushi.top/gtgtgxksfz.html

[E04] 查找子串位置
来源：http://hz.zhoulong.xyz/gtlcgxiszp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yuanzhike.top/gtbkkaqrmd.html

PHP:  strpos($s, "x");
来源：http://hz.shzxlz.cn/gteuzguqwo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yonumen.top/gtxtmpbxmb.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtjgloypka.html

Java: s.indexOf("x")
来源：http://hz.yvedp.cn/gtpojgiivk.html

Go:   strings.Index(s, "x")
来源：http://hz.316326.xyz/gtpeojjhbr.html

Ruby: s.index("x")
来源：http://hz.gzhubu.top/gtupfmomyg.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigfzy.top/gthiziuwjp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zdqjudy.top/gtteishfag.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.feifeiyinyue.top/gtmxjwnkbp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yvedp.cn/gtvrukujms.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sxryk.cn/gtosvaiobj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtzkfawybj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtcfijvtmw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.smart0.xyz/gtdxqvicoq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhoulong.xyz/gtohbpfxzu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gtdgnsqrjo.html

[E06] 替换子串
来源：http://hz.quarkkingdee.top/gtyvyvywmr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.andypj.xyz/gtdvtwvnri.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.fengsongda.top/gtmjcjybkn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtorvhaslr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yuanzhike.top/gteiopcomy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xuanzx.com/gtckatrxku.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtnhojznex.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nanxinkj.top/gtcyxpshqy.html

C#:   s.Replace("a", "b")
来源：http://hz.kuanghao11.cn/gtkiapdzeb.html

[E07] 按分隔符拆分
来源：http://hz.tanke756.top/gtjjgtgxfa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shangyingyoupin.top/gtptwgfjri.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangdashe.top/gtjbxnvomj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtlgvbvaws.html

TS:   s.split(",")
来源：http://hz.nanxinkj.top/gtathtekoc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daria6918.cn/gtigxtdkgs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhaomingkeji.xyz/gtbijxjqux.html

Ruby: s.split(",");  s.split
来源：http://hz.bjfxy.top/gtchqjybvq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.quarkkingdee.top/gtpzkujmjt.html

[E08] 数组按分隔符合并
来源：http://hz.tianlin.xyz/gtdzcttnkm.html

Py:   ",".join(items)
来源：http://hz.gotoacloud.top/gtwwlvgqqc.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtknapbtdn.html

JS:   items.join(",")
来源：http://hz.gotoacloud.top/gtjknrmiku.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gtpniervul.html

Java: String.join(",", items)
来源：http://hz.svipenyu.cn/gtygmeoqlr.html

Go:   strings.Join(items, ",")
来源：http://hz.zhongyouzk.top/gtxspvbytx.html

Ruby: items.join(",")
来源：http://hz.xziqi.cn/gtgeglwysv.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtanxndvdh.html

[E09] 去除所有空白字符
来源：http://hz.guowangkeji.top/gtcbhpuazh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yvedp.cn/gtomaxvaem.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhengqikj.top/gtgsgawdsp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtemiljlkt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.redwolf501.top/gtzxihjxci.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.daria6918.cn/gtbssyivys.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.9152youxi.cn/gtkmvzrgbv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dianchejie.cn/gtcktuyjae.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ivvv.top/gthacwrhuu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yonumen.top/gtnckesxhl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinyuanbaomall.cn/gtbzmifefz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxinkj.top/gttrkvbdky.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtwtpdhaww.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtewieoawn.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtomwdkfpv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtezyrxwml.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gtvjrnyyfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xinyue.icu/gthbeukmrv.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtrrtupbqa.html

Py:   s[::-1]
来源：http://hz.quarkkingdee.top/gtewtuxugz.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gtrfidsxoh.html

JS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtwvneigqi.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtsrnozuqy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xylfe.cn/gtqeheqrxd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xingfuxueyuan.xyz/gteegyunsp.html

Ruby: s.reverse
来源：http://hz.xingfuxueyuan.xyz/gtvulpfiys.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.316326.xyz/gtzfxsyrwq.html

[E12] 统计某字符出现次数
来源：http://hz.xinyue.icu/gtqpldxkve.html

Py:   s.count("a")
来源：http://hz.gogol.net.cn/gtutxevpiu.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangtech.top/gtuebckcwu.html

JS:   s.split("a").length - 1
来源：http://hz.nwbrower.top/gtzmnraxyc.html

TS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtxyzzynfb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtaxcvkxen.html

Go:   strings.Count(s, "a")
来源：http://hz.jinghuilouyu.cn/gtkrnpqpgd.html

Ruby: s.count("a")
来源：http://hz.jiagoushi.top/gtovtioein.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ywan-chungtsiang.top/gtaewitfzu.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtvkungeek.html

Py:   for ch in s: print(ch)
来源：http://hz.52xcode.cn/gtkardabtd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinyuanbaomall.cn/gtmmzxlhxo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtewbvvvkj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.feifeiyinyue.top/gthlxmvrhv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gthwfxjodu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yj20258.top/gthhkxboyl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhongyouzk.top/gtokiofiho.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.xuanzx.com/gtbypxegsd.html

[E14] URL 编码与 Base64
来源：http://hz.shuidangran.top/gtrywvcrkl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.316326.xyz/gtyzlsflyy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yonumen.top/gtilrcbcos.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sufxvd.cn/gtzndvqdgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jiagoushi.top/gtmlifsjdc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aibaodan.cn/gtjdyvuwbd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gzhubu.top/gtudvfefti.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxinkj.top/gtviowxxfl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.52xcode.cn/gtrogzelnc.html

[E15] HTML 转义 / 反转义
来源：http://hz.nanxinkj.top/gtoqknouah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ivvv.top/gtrreruqqe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnqzz.top/gtippozvyw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtslmeamsf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cqqwz.cn/gtirplryhd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.bjfxy.top/gtsrqorgcu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zycfv.cn/gtnwhooukf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xziqi.cn/gtnholafyr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xingfuxueyuan.xyz/gtfvbrxpjc.html

[E16] 数字千分位
来源：http://hz.pengpengdd.cyou/gtglhlfldp.html

Py:   f"{1234567:,}"
来源：http://hz.haohaochexian.top/gtgwfjkdzj.html

PHP:  number_format(1234567);
来源：http://hz.vqdsnc.cn/gtexqhzavi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtofjtdarn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtzkoipcpn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtwnaqhebx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.smart0.xyz/gtmonupimc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gthaeazmob.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtvftttcsh.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtejigrsoh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj202588.top/gtuifbwpxe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinyuanbaomall.cn/gtdvnxkpdx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtzgtxbdhm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.redwolf501.top/gtmbgaurng.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.tianlin.xyz/gtnzrvgnzo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhixingplan.top/gtqsveuobv.html

Ruby: s.capitalize
来源：http://hz.smart0.xyz/gttftigjml.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.ybcxt.top/gtdmchgomg.html

[E18] 模板占位符替换
来源：http://hz.zhoulong.xyz/gtglqyufbq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtvqcjhdsi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenjidiqi.icu/gtowhogpkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigfzy.top/gthtwtipbz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtmxydbiyw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.ydjk.org.cn/gtjdnolyyc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guannengcc.top/gtjojgdwjg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigfzy.top/gtslecejfq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.nanxinkj.top/gtlrjdvfbh.html

[E19] 多行文本按行拆分
来源：http://hz.yuanzhike.top/gtxjdkcsbb.html

Py:   s.splitlines()
来源：http://hz.tanke756.top/gtgvubtlzn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sweek.top/gtfnfxitcp.html

JS:   s.split(/\r?\n/)
来源：http://hz.cashguo.top/gtgkzmjmfy.html

TS:   s.split(/\r?\n/)
来源：http://hz.xinyue.icu/gtzylotrne.html

Java: s.lines().toList()
来源：http://hz.gotoacloud.top/gtuhdvuxcj.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnqzz.top/gtnwsbjmmp.html

Ruby: s.lines
来源：http://hz.ywan-chungtsiang.top/gtgfaeyodr.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtpkijbagn.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtpkhkpqoq.html

Py:   if not s:
来源：http://hz.0kj1m.cn/gtsnwrqwet.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.cucudq.cn/gthpxxrhxl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtounpzkkk.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangtech.top/gtgalndfsk.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigufen.top/gtlxbcwfej.html

Go:   if s == "" {}
来源：http://hz.bjfxy.top/gtuwhnujrz.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtvscadvyq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zdqjudy.top/gtsrrulyxf.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtymvktxqc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nanxuanxn.top/gtrkkjayfl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dianchejie.cn/gtvwohuyvn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hammf.cn/gtmkaxlhjq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gthtcbxyjf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtcziqgpfk.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtldjwvdcm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gtyqqxdssk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.sweek.top/gttfflzgzb.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtqqnloncy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.shangyingyoupin.top/gtjlrbbmpx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtrzhdphgt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aizwys.cn/gtassapcxh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtwcyvmbdw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinghuilouyu.cn/gtwmrmpqbu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.daxiang520.top/gtfojouiwc.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuanzhike.top/gtaycaibgb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtnbgwtzjr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtezscbewq.html

F. 文件与目录
来源：http://hz.yongpay.top/gtmpgmktjt.html

================================================================================
来源：http://hz.jqgfzy.top/gtqzznrkzz.html

[F01] 读取整个文件
来源：http://hz.nwbrower.top/gtmxxjcrkj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.iojbl.cn/gtyglrrnel.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yanxiufei.cn/gtgrisuhat.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.aizwys.cn/gtkdbinxtv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtihkeiklr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtvuvuwpue.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtvteylzmx.html

Ruby: File.read("a.txt")
来源：http://hz.yuxming.cn/gtcfjtdgwk.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj202588.top/gtsrilykls.html

[F02] 逐行读取文件
来源：http://hz.ivvv.top/gtnflqteje.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gtzknlfxix.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.sxryk.cn/gtcofwfrwe.html


<!-- 参考信息 -->