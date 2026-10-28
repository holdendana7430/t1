代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gtvncsuprz.html

[D16] 求和与平均值
来源：http://hz.cucudq.cn/gtclgnwpmq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ivvv.top/gtdotmkslu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.quarkkingdee.top/gtxixkzdsz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtgwwimnxa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gthqyirzis.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtmwonqxnm.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtqckuaigt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtmzwtjpbw.html

C#:   list.Sum();  list.Average()
来源：http://hz.yvedp.cn/gtpbstodfa.html

[D17] 最大值与最小值
来源：http://hz.sweek.top/gtkmmqtssp.html

Py:   max(arr);  min(arr)
来源：http://hz.guannengcc.top/gtmdsepsku.html

PHP:  max($arr);  min($arr);
来源：http://hz.sysykeji.top/gtknxjpxxk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gtrvxhkedy.html

TS:   Math.max(...arr);
来源：http://hz.guowangkeji.top/gtqsymwdxk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gttnuukqzc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhaomingkeji.xyz/gtldjdgbcs.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtqmpdnndc.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtczygtswi.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtuzuwligq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gtbskfjhjj.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtnxvwzqny.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gtjlzvbbnp.html

TS:   nested.flat();
来源：http://hz.snrcjt.cn/gtwqlzveix.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.0kj1m.cn/gtvfjqtlto.html

Go:   // 手写双层循环
来源：http://hz.dianchejie.cn/gtchuvmsyq.html

Ruby: nested.flatten
来源：http://hz.fzhhl.top/gtbrbiglrm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dashuyun.cn/gtwkdlifnn.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtactwqcfo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cucudq.cn/gtguydftwx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxuanxn.top/gtapedfyqw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.havefunace.top/gtkvrtmdoa.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pycfn.com/gtmkittkgl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shanyushiyangtech.top/gtrwscjyjx.html

Go:   // 手写 map[string][]T
来源：http://hz.pengpengdd.cyou/gtqdzbhjyl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yangfankeji.com/gtuxvofept.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gtojtojpsk.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gthtaxdldz.html

Py:   Counter(arr)
来源：http://hz.sufxvd.cn/gtpihekwqz.html

PHP:  array_count_values($arr);
来源：http://hz.iojbl.cn/gtlotrlafn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtgkfdeisw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtcqpormli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yvedp.cn/gtdvcrahnd.html

Go:   // 手写 map[T]int
来源：http://hz.wangshuangyany.cn/gtwfhdalgp.html

Ruby: arr.tally
来源：http://hz.daxiang520.top/gtkjlamduu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnxiangtu.top/gtwuymtijm.html

[D21] 判断是否包含某元素
来源：http://hz.jqgfzy.top/gtqftlecba.html

Py:   x in arr
来源：http://hz.cheryme.top/gtdcomcwnk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtkizxrmue.html

JS:   arr.includes(x)
来源：http://hz.zhiwuduotai.top/gtfzqlfgqq.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtpexvbtby.html

Java: list.contains(x)
来源：http://hz.0kj1m.cn/gtrxwcpdwk.html

Go:   slices.Contains(arr, x)
来源：http://hz.hnqzz.top/gtsmnpnfdt.html

Ruby: arr.include?(x)
来源：http://hz.meibo888.top/gthlcabeux.html

C#:   list.Contains(x)
来源：http://hz.zhiwuduotai.top/gtelcentyq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnqzz.top/gtqbcxhyvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jyoumei.cn/gtplmjzrhn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cashguo.top/gtlihtuiue.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ywan-chungtsiang.top/gtotkzejms.html

TS:   [...arr];
来源：http://hz.hywenlv.cn/gtgdpvmjtn.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtenazhgzq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zycfv.cn/gtzyorzwkz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhaomingkeji.xyz/gtevuhbrrb.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gtcvngnsis.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gticyujlrz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj20258.top/gtfqzvmgsn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtuihlvpfk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtqvqwaczx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtvqutwugh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pycfn.com/gtdvkaouxz.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtjhrgzsex.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jyoumei.cn/gtstkasbsd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jyoumei.cn/gtmgfnboei.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuanzx.com/gtnefmjmqn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtkzmjrxfi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.andypj.xyz/gtfzpjombb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhiwuduotai.top/gtojhptvkj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yuxming.cn/gtsthziqzg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.redwolf501.top/gtfimvqjwa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtimdwxorp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.bjfxy.top/gtkvqtfmll.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgfzy.top/gtxpzpxcni.html

[D25] Set 集合去重与交并差
来源：http://hz.daxiang520.top/gtgluodyno.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zycfv.cn/gtfmrpclts.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yvedp.cn/gtcxfixfxu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtulqhqijo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pengpengdd.cyou/gtryehgjed.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtfpvwioxs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hfpthk.cn/gtzwbbmrvo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtlsgheqba.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hysaishi.cn/gtbjfuhksb.html

[D26] 数组转字符串
来源：http://hz.jinyuanbaomall.cn/gtxgliravk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nanxinkj.top/gtqdrcwtwt.html

PHP:  implode(", ", $arr);
来源：http://hz.yj202588.top/gtrinkvqnd.html

JS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtvzuqmmny.html

TS:   arr.join(", ")
来源：http://hz.cucudq.cn/gtqbravedu.html

Java: String.join(", ", list)
来源：http://hz.chenjidiqi.icu/gtuwejtceo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.aizwys.cn/gtygbukibw.html

Ruby: arr.join(", ")
来源：http://hz.nanxuanxn.top/gtgesptvmq.html

C#:   string.Join(", ", list)
来源：http://hz.yvedp.cn/gtyzsfwuny.html

================================================================================
来源：http://hz.yj202588.top/gtfinqaaxm.html

E. 字符串处理
来源：http://hz.wangdashe.top/gtgjftmdhv.html

================================================================================
来源：http://hz.9152youxi.cn/gtbmkqkncg.html

[E01] 拼接字符串
来源：http://hz.aizwys.cn/gtowrysgwt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhijiandao.cn/gtcsgtdbhs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ydjk.org.cn/gtckhdfcuj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jiagoushi.top/gtzrvzkjhe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgufenzy.top/gtrafoaown.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhijiandao.cn/gteyocwzng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258.top/gtgxpsmfyo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gtkelreiuc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.quarkkingdee.top/gtheersgnj.html

[E02] 重复字符串
来源：http://hz.yuxming.cn/gtrjbxzpex.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gtkxvcggbt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.daxiang520.top/gtpniphuws.html

JS:   "ab".repeat(3)
来源：http://hz.52xcode.cn/gtbdmtkysn.html

TS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtexsqmsbg.html

Java: "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtulzmbdou.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jlsjyb.cn/gtianavxrf.html

Ruby: "ab" * 3
来源：http://hz.jyoumei.cn/gtvnzifkoa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dianchejie.cn/gthdxcsvwj.html

[E03] 截取子串
来源：http://hz.daria6918.cn/gtgwwhisde.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtubkblnof.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258.top/gtuictlmor.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gtkhrigvla.html

TS:   s.slice(1, 4)
来源：http://hz.fengsongda.top/gtvlypygso.html

Java: s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtogdcllpt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.aibaodan.cn/gttguwdlvq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tianlin.xyz/gtzvamsjmm.html

C#:   s.Substring(1, 3)
来源：http://hz.mhx1999.top/gtozjopuer.html

[E04] 查找子串位置
来源：http://hz.zdqjudy.top/gtmhrxsycl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtjtsnmydu.html

PHP:  strpos($s, "x");
来源：http://hz.sxryk.cn/gtvujeuwuj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtqkfontqu.html

TS:   s.indexOf("x")
来源：http://hz.chenlongwang.top/gtakxqygyy.html

Java: s.indexOf("x")
来源：http://hz.52xcode.cn/gtluomddzd.html

Go:   strings.Index(s, "x")
来源：http://hz.gotoacloud.top/gtyssakexk.html

Ruby: s.index("x")
来源：http://hz.andypj.xyz/gtykjuemlv.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtmsltcsmp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jiagoushi.top/gtaepitmmu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hywenlv.cn/gtlxxgzfal.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhaomingkeji.xyz/gtmoltlakp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtpqddnmwf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinghuilouyu.cn/gtkxjlrfts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhixingplan.top/gtrfywusyx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cucudq.cn/gtgtrkmtan.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jiagoushi.top/gtgjgaahvb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.snrcjt.cn/gtxxnlbxdr.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtozatasqx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtqevilzpc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.haohaochexian.top/gtvbxgetth.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtkbbiyrcv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shzxlz.cn/gtqrxzrkzz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtcxnuesph.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xinyue.icu/gtfibbvdik.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gtecxvmboc.html

C#:   s.Replace("a", "b")
来源：http://hz.chenlongwang.top/gtecdzrhms.html

[E07] 按分隔符拆分
来源：http://hz.jyoumei.cn/gtqvmtfsrn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinyuanbaomall.cn/gttgtdxbsa.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj202588.top/gtrioaoscz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hongshengwenyu.top/gteqrhfpkw.html

TS:   s.split(",")
来源：http://hz.zdqjudy.top/gtkkjounql.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtwafegpza.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhaomingkeji.xyz/gtiiinhntg.html

Ruby: s.split(",");  s.split
来源：http://hz.yangfankeji.com/gtbzlhanak.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hnqzz.top/gtgscsmwkm.html

[E08] 数组按分隔符合并
来源：http://hz.zhixingplan.top/gtirueouin.html

Py:   ",".join(items)
来源：http://hz.pycfn.com/gtsfnmtrtp.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtyqggydqp.html

JS:   items.join(",")
来源：http://hz.guowangkeji.top/gtokgjmfbo.html

TS:   items.join(",")
来源：http://hz.zycfv.cn/gtwlupbyfc.html

Java: String.join(",", items)
来源：http://hz.zhoulong.xyz/gtusjqxwck.html

Go:   strings.Join(items, ",")
来源：http://hz.yuanzhike.top/gtiioezyxb.html

Ruby: items.join(",")
来源：http://hz.vqdsnc.cn/gtnhkgnrtd.html

C#:   string.Join(",", items)
来源：http://hz.hywenlv.cn/gtatxrnmlq.html

[E09] 去除所有空白字符
来源：http://hz.dashuyun.cn/gtvkhhtbpv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gtgjcssuoq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.sufxvd.cn/gtfstvfsid.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtretvntga.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtycaaolrl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258.top/gtfxleuvld.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ehwqpu.com/gtgwrkkjlm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.andypj.xyz/gtdjrtqdtr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhiwuduotai.top/gtxocejrir.html

[E10] 左侧补零 / 定长填充
来源：http://hz.haohaochexian.top/gtwktvrzha.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fengsongda.top/gtiyztwhtv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinqigfzy.top/gtsfludenc.html

JS:   "7".padStart(3, "0")
来源：http://hz.jyoumei.cn/gtbtdyrxmd.html

TS:   "7".padStart(3, "0")
来源：http://hz.yonumen.top/gtcrymzqxz.html

Java: String.format("%03d", 7)
来源：http://hz.ppjwa.cn/gtkuxhzpcq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.316326.xyz/gtfhgeqwzq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtonqhwpdl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ywan-chungtsiang.top/gtqrswbzmx.html

[E11] 反转字符串
来源：http://hz.vqdsnc.cn/gtzercnavs.html

Py:   s[::-1]
来源：http://hz.hnxiangtu.top/gtadyfgunc.html

PHP:  strrev($s);
来源：http://hz.ehwqpu.com/gtcvfbvbfl.html

JS:   [...s].reverse().join("")
来源：http://hz.yvedp.cn/gtmwplrpav.html

TS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtnivxewuw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hnqzz.top/gtnlchbgtg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtpdsnhxip.html

Ruby: s.reverse
来源：http://hz.haohaochexian.top/gtbjdnfqwn.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.52xcode.cn/gttbpqzfrd.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtgxsgoqky.html

Py:   s.count("a")
来源：http://hz.tianlin.xyz/gtmmjpbdtw.html

PHP:  substr_count($s, "a");
来源：http://hz.yueranfly.top/gtsaaifkjx.html

JS:   s.split("a").length - 1
来源：http://hz.cheryme.top/gtggjnphir.html

TS:   s.split("a").length - 1
来源：http://hz.jqgufenzy.top/gthbhtmkcf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.aizwys.cn/gtteodkdwb.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtvtwakcbv.html

Ruby: s.count("a")
来源：http://hz.zhijiandao.cn/gtmskeehlr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.c1oappe.top/gttturwjho.html

[E13] 逐字符遍历
来源：http://hz.xylfe.cn/gtoertkzal.html

Py:   for ch in s: print(ch)
来源：http://hz.wangshuangyany.cn/gtpfkhgfvc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.nanxinkj.top/gtrkejbxvt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shzxlz.cn/gtqpuccebh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.haohaochexian.top/gtdyltprgv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tian-w.cn/gtfpnxdaiy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jiagoushi.top/gtkdcaexta.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gthehavdve.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuanzhike.top/gtqyewgody.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258.top/gtbvsvxssj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sysykeji.top/gtanvbkndj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.9152youxi.cn/gtttxtukis.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtcylpdaax.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.0kj1m.cn/gtkdlbmjka.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hnqzz.top/gtzsjddzoa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtlfqtepts.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigfzy.top/gtcblvwhbm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.pengpengdd.cyou/gtjvvuwgjl.html

[E15] HTML 转义 / 反转义
来源：http://hz.jinyuanbaomall.cn/gtnajcotso.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jyoumei.cn/gthszfeelu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yangfankeji.com/gtijyaqhin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tian-w.cn/gtqkcplieg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shzxlz.cn/gtlawgngbu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zhengqikj.top/gtqwntzaiy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtwlrieraz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.vqdsnc.cn/gthbhkzdqb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhijiandao.cn/gtexzszuhm.html

[E16] 数字千分位
来源：http://hz.shangyingyoupin.top/gtcfnpxvit.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gtgxblajfk.html

PHP:  number_format(1234567);
来源：http://hz.daria6918.cn/gtkfhthmni.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtxjmarixk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gtcqjkvyfq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtwkjtnjuc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydzc1.top/gtqmvzjprb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.c1oappe.top/gtacrcshlr.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtyciqjpiv.html

[E17] 首字母大写
来源：http://hz.fzhhl.top/gtovfqxfxe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.haohaochexian.top/gtvjsafmae.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuxming.cn/gtsuejypdu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.nanxuanxn.top/gtaswqffzu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jyoumei.cn/gtylqpbvyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gogol.net.cn/gtvetpxxqv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.birdmap.top/gtrohicoww.html

Ruby: s.capitalize
来源：http://hz.cashguo.top/gtgtqfxonl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.fengsongda.top/gtchnehrks.html

[E18] 模板占位符替换
来源：http://hz.ivvv.top/gtkgnjfeut.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtfdxiufxc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinqigfzy.top/gtjkltpeoz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gthaxnthwr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtawscfwyr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yonumen.top/gtoxqncwfd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtnxztxyzz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hysaishi.cn/gtvmnwugxf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgfzy.top/gtqspzqxgo.html

[E19] 多行文本按行拆分
来源：http://hz.wangdashe.top/gttrdkepfq.html

Py:   s.splitlines()
来源：http://hz.sweek.top/gtagijveio.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ywan-chungtsiang.top/gtgjzxdrsc.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuetiantiany.cn/gtnubodrpd.html

TS:   s.split(/\r?\n/)
来源：http://hz.sysykeji.top/gtkodvxhiv.html

Java: s.lines().toList()
来源：http://hz.vqdsnc.cn/gtbxzgkzkb.html

Go:   strings.Split(s, "\n")
来源：http://hz.ywan-chungtsiang.top/gtmycdfjct.html

Ruby: s.lines
来源：http://hz.zhijiandao.cn/gtvzxipchp.html

C#:   s.Split('\n')
来源：http://hz.chenzaomai.com/gteqqpgwdg.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtirxkjwxv.html

Py:   if not s:
来源：http://hz.yj202588.top/gtrktgonaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.havefunace.top/gtyzgnujkp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hongshengwenyu.top/gtukotsmxf.html

TS:   if (s === "") {}
来源：http://hz.gaohongyu789.top/gtygkdauzz.html

Java: if (s.isEmpty()) {}
来源：http://hz.hnxiangtu.top/gthemzhfbe.html

Go:   if s == "" {}
来源：http://hz.cashguo.top/gtmeidqcdp.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtpglkxsyg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gtuycfaysh.html

[E21] 超长截断加省略号
来源：http://hz.jqgfzy.top/gtvuytjhwm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yj202588.top/gtglzlsjbm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hywenlv.cn/gtafggixcw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtswnodtky.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtxseeherx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtucdbszfj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.316326.xyz/gthpvcagth.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tanke756.top/gtrssuocqe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtxsexljrd.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gtofanzkty.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtirijvfkd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtkaakzkaj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtxmpolymn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhixingplan.top/gtepqudsqo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtvowhbtre.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hysaishi.cn/gtgcmzqrnv.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenzaomai.com/gtcwohzjbv.html


<!-- 参考信息 -->