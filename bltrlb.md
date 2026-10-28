代发 wailian999

C#:   list.Distinct().ToList()
来源：http://hz.yuanzhike.top/gtniuwzclp.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtvooczfse.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pycfn.com/gtvhymixth.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cheryme.top/gtxypwmmsx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtbtdyvuhj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gthbrofcyx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cashguo.top/gtfrhmrffl.html

Go:   // 手写循环累加
来源：http://hz.yvedp.cn/gtgjhdcqhl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xylfe.cn/gtjetynkqg.html

C#:   list.Sum();  list.Average()
来源：http://hz.hongshengwenyu.top/gthcoesxpg.html

[D17] 最大值与最小值
来源：http://hz.guowangkeji.top/gtxdgndmpb.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtcasqltat.html

PHP:  max($arr);  min($arr);
来源：http://hz.xziqi.cn/gtszfjhjbk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sweek.top/gtzpaerals.html

TS:   Math.max(...arr);
来源：http://hz.jlsjyb.cn/gtpnftonnh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtwhagbeth.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtcwhldzxl.html

Ruby: arr.max;  arr.min
来源：http://hz.hammf.cn/gtktrikzfw.html

C#:   list.Max();  list.Min()
来源：http://hz.jinyuanbaomall.cn/gtozjtqvui.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxuanxn.top/gtakoxkflm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jqgufenzy.top/gtgcnlxwig.html

PHP:  array_merge(...$nested);
来源：http://hz.hfpthk.cn/gtdsdvetxe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtuguzyued.html

TS:   nested.flat();
来源：http://hz.kuanghao11.cn/gttxdquwwb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daxiang520.top/gtteqxegiu.html

Go:   // 手写双层循环
来源：http://hz.gzhubu.top/gtcumrefal.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gteljedfey.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.aizwys.cn/gtuizqshea.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtcguqadid.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtsulidyyt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.bjfxy.top/gtvjucajiy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yvedp.cn/gtpyjhhyxq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.mhx1999.top/gtglftafdb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtbezwzwby.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtndqnzley.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hywenlv.cn/gtjtzziyni.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.svipenyu.cn/gtjfpifjdx.html

[D20] 统计每个元素出现次数
来源：http://hz.316326.xyz/gtehmtsxmr.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtkiudbcqk.html

PHP:  array_count_values($arr);
来源：http://hz.fengsongda.top/gtzrgeizly.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtdulzbyai.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtluvlaciw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tian-w.cn/gtgbrwwcdi.html

Go:   // 手写 map[T]int
来源：http://hz.yj20258.top/gtqtujfrhc.html

Ruby: arr.tally
来源：http://hz.hnqzz.top/gtbywmlmph.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.cqqwz.cn/gtkoeagvva.html

[D21] 判断是否包含某元素
来源：http://hz.haohaochexian.top/gtugzosnqn.html

Py:   x in arr
来源：http://hz.jqgufenzy.top/gtbmnaynxo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zycfv.cn/gtirwyolnl.html

JS:   arr.includes(x)
来源：http://hz.xuetiantiany.cn/gtkirvqqzz.html

TS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gtikpgliyw.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtrhwrgbwt.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtkxbnqzhs.html

Ruby: arr.include?(x)
来源：http://hz.yvedp.cn/gtwqodfkqc.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gtqjovkfwn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtoazezvkw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pycfn.com/gtcazzriqy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtmeerirrr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cdnleiting.top/gticqjootx.html

TS:   [...arr];
来源：http://hz.andypj.xyz/gtbsgnemje.html

Java: new ArrayList<>(list);
来源：http://hz.ywan-chungtsiang.top/gtrxrixnfu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtabfrmsgu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.snrcjt.cn/gtsjvrtooi.html

C#:   new List<int>(list);
来源：http://hz.yonumen.top/gtrcfhwgqc.html

[D23] reduce 累积计算
来源：http://hz.cheryme.top/gtnctotazf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.svipenyu.cn/gteizoentb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.wangdashe.top/gtsmotndek.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtwpqphqha.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtietzvylk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gtxejjzazz.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtpndgdgty.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhiwuduotai.top/gtflokxmux.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtvaimhllf.html

[D24] 字典 / Map 基本操作
来源：http://hz.ehwqpu.com/gtblctugmw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gtnkcederl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtlrgsbkca.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.quarkkingdee.top/gtfhjklazh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnqzz.top/gtdnpovozx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sxryk.cn/gtqhwnlyja.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.feifeiyinyue.top/gtprhxeaph.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtwpxcziod.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.c1oappe.top/gtswglmyqn.html

[D25] Set 集合去重与交并差
来源：http://hz.jinyuanbaomall.cn/gtanfenspz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yongpay.top/gtkohuiiez.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hfpthk.cn/gtlpprugtz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtkdvhypac.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtjjdkwszk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fengsongda.top/gtinqejyup.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtxvdzkqxl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tianlin.xyz/gtporabqcp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtdqfzlvwk.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangkeji.top/gtpgyaqgms.html

Py:   ", ".join(map(str, arr))
来源：http://hz.c1oappe.top/gtpncydqrp.html

PHP:  implode(", ", $arr);
来源：http://hz.smart0.xyz/gtkpgbamsi.html

JS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtaexkkhtz.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtenzpcrqt.html

Java: String.join(", ", list)
来源：http://hz.wangdashe.top/gtajdvroyq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shangyingyoupin.top/gtkixosqma.html

Ruby: arr.join(", ")
来源：http://hz.tian-w.cn/gtiorrptrp.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtvhyuloov.html

================================================================================
来源：http://hz.shuidangran.top/gtpyucopji.html

E. 字符串处理
来源：http://hz.hnxiangtu.top/gtrsookqkh.html

================================================================================
来源：http://hz.0kj1m.cn/gtbxihmiql.html

[E01] 拼接字符串
来源：http://hz.havefunace.top/gtwtbparmz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.hfpthk.cn/gtmrgqrhgh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxinkj.top/gtenqswgcb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtragytysi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtgxcrbpai.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.daria6918.cn/gtuhiublai.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hywenlv.cn/gtqwsxoefq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.smart0.xyz/gtdverlbur.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtcsqwaenm.html

[E02] 重复字符串
来源：http://hz.hnqzz.top/gttkpgyags.html

Py:   "ab" * 3
来源：http://hz.jiagoushi.top/gtgrwqxhde.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hongshengwenyu.top/gtyopamyeh.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtgyktbfwi.html

TS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtaqgjfnrj.html

Java: "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtifiumoiv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ivvv.top/gtmtjqoxzj.html

Ruby: "ab" * 3
来源：http://hz.cucudq.cn/gtmmdtsyyn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtliammcqh.html

[E03] 截取子串
来源：http://hz.cashguo.top/gtkbhjiwfe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhoulong.xyz/gtvaowofqb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtlrdczgav.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtxgdljizd.html

TS:   s.slice(1, 4)
来源：http://hz.redwolf501.top/gtdbvebmlc.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gtkpzqsecv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hywenlv.cn/gtnaxuelhw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ydjk.org.cn/gtxqwvbowf.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258.top/gtpsqwowbw.html

[E04] 查找子串位置
来源：http://hz.quarkkingdee.top/gtkqoosixk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shzxlz.cn/gteqhgcxlt.html

PHP:  strpos($s, "x");
来源：http://hz.yonumen.top/gtnambqury.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgfzy.top/gtalzgvvxs.html

TS:   s.indexOf("x")
来源：http://hz.yj20258.top/gtksqpampg.html

Java: s.indexOf("x")
来源：http://hz.aizwys.cn/gtwfjctuya.html

Go:   strings.Index(s, "x")
来源：http://hz.c1oappe.top/gtnpqkiaax.html

Ruby: s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtdjgxthhk.html

C#:   s.IndexOf("x")
来源：http://hz.jinqigufen.top/gtlcrjgduc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shangyingyoupin.top/gtaivdqxjk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.kuanghao11.cn/gteeboekfn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtrmnibvvs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cdnleiting.top/gtvwfuwvog.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtmktitcly.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fengsongda.top/gtvkszicvy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yueranfly.top/gtnnytwhsn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtnwguramm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.iojbl.cn/gtyobektha.html

[E06] 替换子串
来源：http://hz.ppjwa.cn/gtuxrbszzj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.svipenyu.cn/gtkpxdxqop.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.daxiang520.top/gtxbaxclmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtitrcqxbz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ydzc1.top/gtipxsrvvs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtidqqyxpu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cqqwz.cn/gtcdeovbpj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cucudq.cn/gtuwwlhrxd.html

C#:   s.Replace("a", "b")
来源：http://hz.316326.xyz/gtxtwbcaww.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtavquvifp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.wangshuangyany.cn/gttanqxsgp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yj20258888.top/gtsbcxudik.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ydzc1.top/gtifojoewf.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtgmqgcupz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hysaishi.cn/gtizoqjrgl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenzaomai.com/gtusnqyhxb.html

Ruby: s.split(",");  s.split
来源：http://hz.mhx1999.top/gtokabxcbz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cheryme.top/gtshczupbj.html

[E08] 数组按分隔符合并
来源：http://hz.havefunace.top/gtucrgldsg.html

Py:   ",".join(items)
来源：http://hz.nanxinkj.top/gtzvzwwhdd.html

PHP:  implode(",", $items);
来源：http://hz.jinqigfzy.top/gtytcxnxrw.html

JS:   items.join(",")
来源：http://hz.jqgufenzy.top/gtcmmtolhm.html

TS:   items.join(",")
来源：http://hz.gogol.net.cn/gtkyhrcbkz.html

Java: String.join(",", items)
来源：http://hz.xuetiantiany.cn/gtbehetdcm.html

Go:   strings.Join(items, ",")
来源：http://hz.cheryme.top/gtgxsxqugl.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtjwsewffy.html

C#:   string.Join(",", items)
来源：http://hz.meibo888.top/gtvuichabz.html

[E09] 去除所有空白字符
来源：http://hz.pycfn.com/gtzlfvvgbh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.feifeiyinyue.top/gtfuqsenxu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.pengpengdd.cyou/gtkfivfxak.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinyuanbaomall.cn/gtfszcevrh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhoulong.xyz/gtgmjpfnhl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nwbrower.top/gtjinqgukl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtbaavsrhc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yvedp.cn/gtwlgnhial.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenlongwang.top/gtnygnzsgk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.dianchejie.cn/gtxvplbcop.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xziqi.cn/gtxasmfous.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtwatcrioy.html

JS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtsiugockr.html

TS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtbpmghqsy.html

Java: String.format("%03d", 7)
来源：http://hz.gaohongyu789.top/gtwvlrgqby.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtldyqxnjg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtsednwnji.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangkeji.top/gtcveekekk.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtwjmhyigq.html

Py:   s[::-1]
来源：http://hz.yj202588.top/gtjrnpoebo.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gtcyipckub.html

JS:   [...s].reverse().join("")
来源：http://hz.xuetiantiany.cn/gtrmvnvptw.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtvgozuygx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zdqjudy.top/gtcixbgpmq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxinkj.top/gtltchveqm.html

Ruby: s.reverse
来源：http://hz.gotoacloud.top/gtliqahqmr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinghuilouyu.cn/gtzboggzoj.html

[E12] 统计某字符出现次数
来源：http://hz.hongshengwenyu.top/gtduchkpxl.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gtqbuwajbz.html

PHP:  substr_count($s, "a");
来源：http://hz.jinqigufen.top/gtdbiwhrtu.html

JS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtmicrzwya.html

TS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gtkdoxvqrn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sufxvd.cn/gthxugojig.html

Go:   strings.Count(s, "a")
来源：http://hz.jyoumei.cn/gttjcwxdbk.html

Ruby: s.count("a")
来源：http://hz.jqgufenzy.top/gthpvetfzv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sweek.top/gtknabgaji.html

[E13] 逐字符遍历
来源：http://hz.shangyingyoupin.top/gtrajxodod.html

Py:   for ch in s: print(ch)
来源：http://hz.9152youxi.cn/gtzmfagcgz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtgrigmjkm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinyuanbaomall.cn/gtywfdgsrn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuxming.cn/gtcokyfzut.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gotoacloud.top/gtgwdjloas.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zhongyouzk.top/gtcmkgchtg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gtaeyqqfkc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hnxiangtu.top/gtfpfjlire.html

[E14] URL 编码与 Base64
来源：http://hz.zhixingplan.top/gtqfqeevrg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shzxlz.cn/gterumqcok.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ydzc1.top/gtpoqsjwpu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnxiangtu.top/gtyrddbihf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydjk.org.cn/gtvuvnqgso.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtuhdglnjt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.redwolf501.top/gtkswxgjej.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zdqjudy.top/gtlbafjnln.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtawtmxfjh.html

[E15] HTML 转义 / 反转义
来源：http://hz.ehwqpu.com/gtgcaipvsu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.gaohongyu789.top/gttftjhqtj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hysaishi.cn/gtwnpcqwxc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.shzxlz.cn/gtxpywudvj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shzxlz.cn/gtvatkkfxa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sysykeji.top/gtphfmalcv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ywan-chungtsiang.top/gtzzzuilqd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhongyouzk.top/gtiviwhbkl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.snrcjt.cn/gtzsdntpeo.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtsbxtrrfp.html

Py:   f"{1234567:,}"
来源：http://hz.dashuyun.cn/gtitdbbwkw.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gtzkosmqzx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zycfv.cn/gtyyvhjmgc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtsamzydia.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jlsjyb.cn/gtekmyeqje.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gttfcyxxhl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.meibo888.top/gtickxjvah.html

C#:   1234567.ToString("N0")
来源：http://hz.yanxiufei.cn/gtbnrjxflx.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtqpfcftck.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dashuyun.cn/gtppyrnvvg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.feifeiyinyue.top/gtsixrnjhl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yanxiufei.cn/gtpzeiwyew.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xingfuxueyuan.xyz/gtloltxtrd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.svipenyu.cn/gtkscnvgvd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jlsjyb.cn/gtjbaqzayg.html

Ruby: s.capitalize
来源：http://hz.yueranfly.top/gtinshqbby.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtzilproqg.html

[E18] 模板占位符替换
来源：http://hz.guannengcc.top/gtfgrxkaww.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.fengsongda.top/gtemgyjupz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yongpay.top/gtakaeqoel.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtrteggpnr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuanzhike.top/gthfjrylir.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtccytuxmm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dianchejie.cn/gtuyqlaikt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gzhubu.top/gtfnauucyi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtbosxjndd.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtbndrrgju.html

Py:   s.splitlines()
来源：http://hz.0kj1m.cn/gtbjwdbxqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.svipenyu.cn/gtykbgkelw.html

JS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtnbkfslps.html

TS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gthfgvqpoj.html

Java: s.lines().toList()
来源：http://hz.guowangkeji.top/gtadlfipqc.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtqeucmlfe.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtmclyiznb.html

C#:   s.Split('\n')
来源：http://hz.gaohongyu789.top/gtzfmoerdx.html

[E20] 判断字符串是否为空
来源：http://hz.c1oappe.top/gtplqnplrc.html

Py:   if not s:
来源：http://hz.yueranfly.top/gtgxnredae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.wangdashe.top/gtjgikdimi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yangfankeji.com/gtjvzfczan.html

TS:   if (s === "") {}
来源：http://hz.zycfv.cn/gtcpwvhkwh.html

Java: if (s.isEmpty()) {}
来源：http://hz.haohaochexian.top/gthnnuuuvi.html

Go:   if s == "" {}
来源：http://hz.jlsjyb.cn/gtfcziqaoo.html

Ruby: if s.empty?
来源：http://hz.cqqwz.cn/gtxrtoaurb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.meibo888.top/gtzgkuffjx.html

[E21] 超长截断加省略号
来源：http://hz.9152youxi.cn/gtoqfkwhuz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.bjfxy.top/gtshnbjovu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtnqzwcvpa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhijiandao.cn/gtqtwrdvfp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtlegvrzbn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.wangshuangyany.cn/gtjoauhckj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.feifeiyinyue.top/gtubmzyrdq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtmvsprfuo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.mhx1999.top/gtthrmxvfh.html

[E22] 字节长度与字符长度
来源：http://hz.sufxvd.cn/gtprkmzcap.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.havefunace.top/gtbwinkpbf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.sufxvd.cn/gtykatwojy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.sufxvd.cn/gtwpeikcqx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ppjwa.cn/gtbqfpwzlk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hysaishi.cn/gtczbteqpr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinghuilouyu.cn/gtidccyplu.html

Ruby: s.bytesize;  s.length
来源：http://hz.xinyue.icu/gtcnncagdq.html


<!-- 参考信息 -->