代发 wailian999

C#:   list.Reverse();
来源：http://hz.cdnleiting.top/gtsvibvjgb.html

[D12] 查找元素下标
来源：http://hz.zdqjudy.top/gtuppubpfs.html

Py:   arr.index(x);  x in arr
来源：http://hz.jlsjyb.cn/gtbwphfmfw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtljufjbph.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtalxhstbq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtdnagnywc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yvedp.cn/gtulaqbopg.html

Go:   slices.Index(arr, x)
来源：http://hz.chenjidiqi.icu/gtxalvtezk.html

Ruby: arr.index(x)
来源：http://hz.shzxlz.cn/gtdyvhvsfx.html

C#:   list.IndexOf(x);
来源：http://hz.xylfe.cn/gtmfvjtvvl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gthbfmldcy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtazvxnpmp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jlsjyb.cn/gtwqiwrkat.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtdqgselrg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.meibo888.top/gtddydnhgc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtteemkfgc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yuxming.cn/gtixlpwiaw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhiwuduotai.top/gttfmvexli.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhengqikj.top/gtedfesgnc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xylfe.cn/gtkmhwgynw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.feifeiyinyue.top/gtqznylzuo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtxnfzmjsy.html

JS:   arr.map(x => x * 2)
来源：http://hz.feifeiyinyue.top/gthjhuqezz.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtxhdycgue.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtfttajslk.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtzxixiwik.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gotoacloud.top/gtqyuymrbg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.iojbl.cn/gtmvlfxngc.html

[D15] 去重
来源：http://hz.c1oappe.top/gtdosiqyqt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtcqlghvrv.html

PHP:  array_unique($arr);
来源：http://hz.chenzaomai.com/gtzgfurqvp.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gthyrpsqot.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtqeujlole.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtrrhnbaix.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtmzwhqccg.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtoismumom.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gtpanojoma.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtlojusciq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtlfnfhgzz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sufxvd.cn/gtjcioqpqa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtcnobyqgv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtmtynmsvr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenjidiqi.icu/gtbkzbvivi.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtpmwpvrud.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.feifeiyinyue.top/gtxaftziwj.html

C#:   list.Sum();  list.Average()
来源：http://hz.gogol.net.cn/gtvhgdvzdb.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtapmuhwxo.html

Py:   max(arr);  min(arr)
来源：http://hz.shuidangran.top/gtnrikqvwi.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gtbrqnszyn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtkrbowqsx.html

TS:   Math.max(...arr);
来源：http://hz.svipenyu.cn/gtgmsfruze.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtrsbpeqbe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shanyushiyangtech.top/gttkcksxvr.html

Ruby: arr.max;  arr.min
来源：http://hz.shangyingyoupin.top/gtdgthxqal.html

C#:   list.Max();  list.Min()
来源：http://hz.shanyushiyangkeji.top/gtcvpyqpcj.html

[D18] 扁平化嵌套数组
来源：http://hz.birdmap.top/gteyjbddce.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.bjfxy.top/gtgzvqqqxu.html

PHP:  array_merge(...$nested);
来源：http://hz.cqqwz.cn/gtwrveiofi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.0kj1m.cn/gtoplvtsqm.html

TS:   nested.flat();
来源：http://hz.aibaodan.cn/gtzxwguyiw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.aizwys.cn/gtehdukjgc.html

Go:   // 手写双层循环
来源：http://hz.xingfuxueyuan.xyz/gtnohddlth.html

Ruby: nested.flatten
来源：http://hz.zhengqikj.top/gtunbmtgqv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtskkakcin.html

[D19] 按字段分组
来源：http://hz.c1oappe.top/gtgihlgpjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gthdrvzpfa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shangyingyoupin.top/gtsbsheelt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.gzhubu.top/gtyvznlzrg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yj202588.top/gtnozkvmyc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtwphjyobp.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtozmcwxjs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtiernoedn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtzqxsnnhs.html

[D20] 统计每个元素出现次数
来源：http://hz.hfpthk.cn/gtomimklxo.html

Py:   Counter(arr)
来源：http://hz.zhaomingkeji.xyz/gtyjrsvrgq.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtpgtwvgxc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtwhvplvsn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtzndwoaxn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pycfn.com/gtbayhezde.html

Go:   // 手写 map[T]int
来源：http://hz.9152youxi.cn/gttzvwjinc.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtzxbvizua.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.bjfxy.top/gtaahqkypd.html

[D21] 判断是否包含某元素
来源：http://hz.nwbrower.top/gtobwlftjh.html

Py:   x in arr
来源：http://hz.kuanghao11.cn/gtemzkcokl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gtxeskggyq.html

JS:   arr.includes(x)
来源：http://hz.fengsongda.top/gtljcjmamc.html

TS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtelsnitak.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtxyzgigxj.html

Go:   slices.Contains(arr, x)
来源：http://hz.sysykeji.top/gtovojlxmj.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtxjrqnubg.html

C#:   list.Contains(x)
来源：http://hz.yj202588.top/gtjaidetbq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sxryk.cn/gtktnqqfet.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hnqzz.top/gtixavwksv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.kuanghao11.cn/gtpsezczpw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtxfqkagfl.html

TS:   [...arr];
来源：http://hz.wangdashe.top/gtcmmfwazx.html

Java: new ArrayList<>(list);
来源：http://hz.quarkkingdee.top/gtcpjsvrcq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gthwfcyvwf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtwmpjnywa.html

C#:   new List<int>(list);
来源：http://hz.quarkkingdee.top/gtdyrbjrkj.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gtumajnttd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tanke756.top/gtvjdjtujn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gzhubu.top/gtdqzvtvlr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gtcgacqxle.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtzvgpckux.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtjxosvgfu.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtcxibxvbb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gtexnhkuld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yuxming.cn/gthojdfery.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtmkbzoyzl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtvqlwezqp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.gzhubu.top/gtrovxetlb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yanxiufei.cn/gtmtlwznlz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cashguo.top/gtcckljspb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtzmcizudr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ivvv.top/gtqowksofo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aibaodan.cn/gtxxtmcpsi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinghuilouyu.cn/gtydaklcsr.html

[D25] Set 集合去重与交并差
来源：http://hz.nanxuanxn.top/gtsjsmawbz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxinkj.top/gtyxyvyevl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yj20258888.top/gtpnigkuph.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtmchqtojp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtybwyypwc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhongyouzk.top/gtpstrwoai.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jianghu66.top/gtkoyghkds.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtfleygnyf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.fengsongda.top/gtsazmipjo.html

[D26] 数组转字符串
来源：http://hz.52xcode.cn/gtjcrasewr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhongyouzk.top/gtlyjmxgmn.html

PHP:  implode(", ", $arr);
来源：http://hz.haohaochexian.top/gtkuasusfr.html

JS:   arr.join(", ")
来源：http://hz.yj202588.top/gtccbctzej.html

TS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtalzhqbwx.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtqhmqmwje.html

Go:   strings.Join(strs, ", ")
来源：http://hz.meibo888.top/gtptgglvgf.html

Ruby: arr.join(", ")
来源：http://hz.havefunace.top/gtlpipvjop.html

C#:   string.Join(", ", list)
来源：http://hz.gogol.net.cn/gtpjwadkti.html

================================================================================
来源：http://hz.fengsongda.top/gtixcnkqzo.html

E. 字符串处理
来源：http://hz.316326.xyz/gtdqzxssot.html

================================================================================
来源：http://hz.ivvv.top/gthcuexhmw.html

[E01] 拼接字符串
来源：http://hz.tian-w.cn/gtljixizsp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtwuzwfksm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtjkkdgsvq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtllyqbxbe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gthzzoyluu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtaemqcuci.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jqgufenzy.top/gtidcwprls.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nwbrower.top/gtwnpkumvu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhiwuduotai.top/gtpwymnavn.html

[E02] 重复字符串
来源：http://hz.chenzaomai.com/gtltzaqrlp.html

Py:   "ab" * 3
来源：http://hz.shangyingyoupin.top/gtfddbkicn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jianghu66.top/gtarlfkwkv.html

JS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtltsgkkwn.html

TS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtgoxtwtex.html

Java: "ab".repeat(3)
来源：http://hz.shuidangran.top/gtykehosnx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtqprpecki.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtttpxtolp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtxoixvfoz.html

[E03] 截取子串
来源：http://hz.hywenlv.cn/gtnnaybvth.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gtowegfxrp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nwbrower.top/gtmrehgmxb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtvjwyslbw.html

TS:   s.slice(1, 4)
来源：http://hz.tianlin.xyz/gtmxxrxewj.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtpyqlgjht.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gtevzfkzkc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtqzgblxly.html

C#:   s.Substring(1, 3)
来源：http://hz.jinghuilouyu.cn/gtwpihltml.html

[E04] 查找子串位置
来源：http://hz.cucudq.cn/gtutbkwrod.html

Py:   s.find("x");  s.index("x")
来源：http://hz.c1oappe.top/gtdolvphsr.html

PHP:  strpos($s, "x");
来源：http://hz.nanxuanxn.top/gtfqoupzxl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhiwuduotai.top/gtumvxenkf.html

TS:   s.indexOf("x")
来源：http://hz.guannengcc.top/gtwbduuvcc.html

Java: s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtzwalnczp.html

Go:   strings.Index(s, "x")
来源：http://hz.ywan-chungtsiang.top/gtynwchuke.html

Ruby: s.index("x")
来源：http://hz.fengsongda.top/gttfcjgvcx.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtffmqitkk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.c1oappe.top/gturocvpkh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gtgsdsufzc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daria6918.cn/gtgytgtgvp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtojpiyely.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shanyushiyangtech.top/gtogdqthcw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtzvllbbbn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigufen.top/gtvbvwjorx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yongpay.top/gtxxwuoawr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gttugnmlhr.html

[E06] 替换子串
来源：http://hz.gaohongyu789.top/gtgmlqfgfu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tianlin.xyz/gtouewntzh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxuanxn.top/gtvhonqkrv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtngmmgnpl.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtkctvtmgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtabvztbdd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daria6918.cn/gtnxvesafc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtffovlcfu.html

C#:   s.Replace("a", "b")
来源：http://hz.hywenlv.cn/gtlbnzesbt.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gthakygqjs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258.top/gtryjaodkz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.sweek.top/gtdrrjjpib.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sysykeji.top/gtxvppkpcw.html

TS:   s.split(",")
来源：http://hz.316326.xyz/gtlawlcodn.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yanxiufei.cn/gtbikwrrzn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zdqjudy.top/gteupqflot.html

Ruby: s.split(",");  s.split
来源：http://hz.yvedp.cn/gtmpjsbqmh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.meibo888.top/gttxkhreur.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtbebnchbs.html

Py:   ",".join(items)
来源：http://hz.yangfankeji.com/gtpxfjdrdc.html

PHP:  implode(",", $items);
来源：http://hz.guowangkeji.top/gtsgucacwx.html

JS:   items.join(",")
来源：http://hz.xziqi.cn/gtvsqnjzek.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtkkzkxdxv.html

Java: String.join(",", items)
来源：http://hz.shzxlz.cn/gtkmlfntgh.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtvkzqrxut.html

Ruby: items.join(",")
来源：http://hz.hysaishi.cn/gtzhfyvzin.html

C#:   string.Join(",", items)
来源：http://hz.yuanzhike.top/gtcycgtpsz.html

[E09] 去除所有空白字符
来源：http://hz.yuanzhike.top/gtrdxjumae.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.feifeiyinyue.top/gtszgbfnxz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.haohaochexian.top/gtooapyrtq.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtqnbivezl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtgkvzzaox.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.havefunace.top/gthyfifetz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cqqwz.cn/gtqfqkefsh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.svipenyu.cn/gtxczskhqm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtmbsinuav.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hammf.cn/gtwcytfvlk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.birdmap.top/gttiaiuayq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtififsobt.html

JS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtlksmkcgn.html

TS:   "7".padStart(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtnlfgtdoi.html

Java: String.format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtbpwneazs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.smart0.xyz/gtvynfptbw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtsswqjsqb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.svipenyu.cn/gtimblipcy.html

[E11] 反转字符串
来源：http://hz.daxiang520.top/gtqfrfeqin.html

Py:   s[::-1]
来源：http://hz.0kj1m.cn/gtezuduhwi.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtxufwsulc.html

JS:   [...s].reverse().join("")
来源：http://hz.cheryme.top/gtgluavttu.html

TS:   [...s].reverse().join("")
来源：http://hz.hysaishi.cn/gtuxypeuel.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.nanxinkj.top/gtoirszpue.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gogol.net.cn/gttcnliyto.html

Ruby: s.reverse
来源：http://hz.wangdashe.top/gtprijyboz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtkublmiuz.html

[E12] 统计某字符出现次数
来源：http://hz.yanxiufei.cn/gtekycevkb.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtqvzbxxmx.html

PHP:  substr_count($s, "a");
来源：http://hz.yvedp.cn/gtfocehvdv.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gtbvgpbalg.html

TS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtexhvvknf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yvedp.cn/gtfanorito.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtmktwnwrn.html

Ruby: s.count("a")
来源：http://hz.jinyuanbaomall.cn/gttedhjqlt.html

C#:   s.Count(c => c == 'a')
来源：http://hz.sysykeji.top/gtdzjbegst.html

[E13] 逐字符遍历
来源：http://hz.zhengqikj.top/gtrcbmvwmi.html

Py:   for ch in s: print(ch)
来源：http://hz.gzhubu.top/gtiiamdmlr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jinqigfzy.top/gtlkfnbtbe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtygilqfso.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhoulong.xyz/gtapnwdysh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhengqikj.top/gtwdffuych.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shuidangran.top/gtknrjpgxl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gzhubu.top/gtzfavuzmo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.smart0.xyz/gtzjtgqzpf.html

[E14] URL 编码与 Base64
来源：http://hz.smart0.xyz/gtsefacbqf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gtnvrsvyhr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hfpthk.cn/gthabvhyiw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.meibo888.top/gtcosapxaw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinyuanbaomall.cn/gtdbtmaypq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtwjeqpnzq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ppjwa.cn/gtknoibuuc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hysaishi.cn/gtkewqnlna.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.snrcjt.cn/gtyzfnqwaf.html

[E15] HTML 转义 / 反转义
来源：http://hz.redwolf501.top/gtsyyqlshy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.andypj.xyz/gtasrfmfuh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.bjfxy.top/gtwhavkxdu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.nwbrower.top/gthdjcaeio.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtoshhokaa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cucudq.cn/gtvkfoxjpg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.havefunace.top/gtbsbgevyt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.0kj1m.cn/gtupbhmamv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtxdhsfihj.html

[E16] 数字千分位
来源：http://hz.hysaishi.cn/gtmcdxarwu.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtgslwvuoy.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtarsjhrbj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtujlapeqa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtaaaukjap.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.kuanghao11.cn/gteicgitts.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtqeqodnmn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj202588.top/gtvbphfcel.html

C#:   1234567.ToString("N0")
来源：http://hz.yonumen.top/gtqmcayzzz.html

[E17] 首字母大写
来源：http://hz.iojbl.cn/gtxudwrmwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shanyushiyangtech.top/gtickmaiat.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shzxlz.cn/gternqovgm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cheryme.top/gtgoqvbwcd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shanyushiyangkeji.top/gtayvicdib.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gtovzuoppk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shanyushiyangtech.top/gtgbpfkpst.html

Ruby: s.capitalize
来源：http://hz.hnxiangtu.top/gtrynduxft.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtgfdxmwtx.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtcvncldhz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.9152youxi.cn/gtntksnwzu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuanzx.com/gtqwuuetdd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sufxvd.cn/gtrxknvyfu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.guannengcc.top/gtoahlzemc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnqzz.top/gtkdgcmgwg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xingfuxueyuan.xyz/gtgpgmcomf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shangyingyoupin.top/gtowublmna.html


<!-- 参考信息 -->