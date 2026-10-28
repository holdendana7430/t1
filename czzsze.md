代发 wailian999

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtrhvktsbx.html

Java: Collections.reverse(list);
来源：http://hz.guowangkeji.top/gttmwklvgp.html

Go:   slices.Reverse(arr)
来源：http://hz.daxiang520.top/gtzsazeret.html

Ruby: arr.reverse
来源：http://hz.zdqjudy.top/gtbknsfdmo.html

C#:   list.Reverse();
来源：http://hz.yuanzhike.top/gtxjfmrvhe.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtvrasmngy.html

Py:   arr.index(x);  x in arr
来源：http://hz.feifeiyinyue.top/gtgzhpubzl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtalvsppsc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtwqbnkbnz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtuuoapybe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.tianlin.xyz/gtvfyquuwf.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtghoifqgc.html

Ruby: arr.index(x)
来源：http://hz.yueranfly.top/gtyvzlrdml.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtuyilmbub.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yanxiufei.cn/gtmqfsevws.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.fengsongda.top/gthgdmmssp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shuidangran.top/gttzwapgtb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xylfe.cn/gtkddjrvsl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nwbrower.top/gtjuluvoiw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hysaishi.cn/gtbgbqzoal.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuetiantiany.cn/gtkxbgupqt.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangkeji.top/gtilwuntaf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cheryme.top/gtogmxctsq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sufxvd.cn/gtvijpjomb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtzajtvgjj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gtezgwnjib.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtdbittjsf.html

TS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtterprrtk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gtnquabsxu.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtczkxhpea.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtypigkwpv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hysaishi.cn/gttesdnrul.html

[D15] 去重
来源：http://hz.ehwqpu.com/gtsemgcovj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenlongwang.top/gtwjojozui.html

PHP:  array_unique($arr);
来源：http://hz.snrcjt.cn/gtcwiqynju.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtpwwqtauy.html

TS:   [...new Set(arr)]
来源：http://hz.tian-w.cn/gtbwjherpc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinqigufen.top/gtoivnakul.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtyzwtapux.html

Ruby: arr.uniq
来源：http://hz.birdmap.top/gtvjlpuyii.html

C#:   list.Distinct().ToList()
来源：http://hz.mhx1999.top/gtptxipqbc.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtjmmijhup.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yangfankeji.com/gtbsbtzuji.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.kuanghao11.cn/gtxdmijqpx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gticohnfvg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.quarkkingdee.top/gtjzpmwdub.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnqzz.top/gtjenxomws.html

Go:   // 手写循环累加
来源：http://hz.dianchejie.cn/gtenfnjatl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhoulong.xyz/gtzpmmxoej.html

C#:   list.Sum();  list.Average()
来源：http://hz.pycfn.com/gttnppgmqk.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtttqjwvvz.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtkeervvlr.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtmrdpjyro.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yongpay.top/gtgyhwsdci.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gthbdxoamh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.quarkkingdee.top/gtnkeqevnl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtvgewxiko.html

Ruby: arr.max;  arr.min
来源：http://hz.andypj.xyz/gtkolllila.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtfelyvwfc.html

[D18] 扁平化嵌套数组
来源：http://hz.birdmap.top/gtqvxynnyg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuxming.cn/gtjqfvszfl.html

PHP:  array_merge(...$nested);
来源：http://hz.ppjwa.cn/gtiijujrno.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jyoumei.cn/gtskbnarxi.html

TS:   nested.flat();
来源：http://hz.pengpengdd.cyou/gtulutawhz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hammf.cn/gtyrueygha.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtekrmsslc.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gtwxewbqky.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.andypj.xyz/gtqcyeowhw.html

[D19] 按字段分组
来源：http://hz.sxryk.cn/gtbamqejht.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtnfbbijdq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gtzxpaehtw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.iojbl.cn/gtndduaigk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtszwqrzqw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.vqdsnc.cn/gtpziznxgu.html

Go:   // 手写 map[string][]T
来源：http://hz.bjfxy.top/gtyqrjrwcf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gteqnzpjzf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pycfn.com/gtuaxhqnxo.html

[D20] 统计每个元素出现次数
来源：http://hz.hysaishi.cn/gtvwsgawdy.html

Py:   Counter(arr)
来源：http://hz.0kj1m.cn/gtdxrfkdpb.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtgmpybods.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gttjygvjow.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtdkbqnaap.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinqigfzy.top/gtlfruygfw.html

Go:   // 手写 map[T]int
来源：http://hz.tianlin.xyz/gthomjexmf.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtxadtbebf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxuanxn.top/gtwqxolmka.html

[D21] 判断是否包含某元素
来源：http://hz.yj20258888.top/gtqiojodzo.html

Py:   x in arr
来源：http://hz.tian-w.cn/gtgznxydoh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gzhubu.top/gtbfppdqnf.html

JS:   arr.includes(x)
来源：http://hz.tanke756.top/gtoylyvivy.html

TS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtmprmfsxc.html

Java: list.contains(x)
来源：http://hz.zhijiandao.cn/gtnnpbjedu.html

Go:   slices.Contains(arr, x)
来源：http://hz.shzxlz.cn/gtzfqobrli.html

Ruby: arr.include?(x)
来源：http://hz.haohaochexian.top/gtftykfepn.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtqvwnnyqd.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtjbwhdzmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zycfv.cn/gtbssqycwu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtpfkojpoh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangtech.top/gtgtttyptt.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtmcpoctcj.html

Java: new ArrayList<>(list);
来源：http://hz.gaohongyu789.top/gtmcadskgu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.bjfxy.top/gtfksernmi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shuidangran.top/gtufrfzaiw.html

C#:   new List<int>(list);
来源：http://hz.zhaomingkeji.xyz/gtfttfwnah.html

[D23] reduce 累积计算
来源：http://hz.sysykeji.top/gteuiubfhn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtyymqffja.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jlsjyb.cn/gtljoaqrlp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtwyxkheyd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtmlmcaeml.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydzc1.top/gtipjjnrgy.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtmwofglmr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.0kj1m.cn/gthyjcggui.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sufxvd.cn/gtxrfjmomr.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtpmphlvug.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jyoumei.cn/gtnvmlcgld.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtypjdxtmv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sysykeji.top/gtylatcbec.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtnovgkfpc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtmvsipkfc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gtsxenxpwl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenzaomai.com/gtpfswoged.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.xylfe.cn/gtljmjtogy.html

[D25] Set 集合去重与交并差
来源：http://hz.hongshengwenyu.top/gtkofmofcf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ehwqpu.com/gtsemetqot.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.tanke756.top/gtdkhrglyc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cheryme.top/gtjimtzmvv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtlspssjil.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtzgvzoeom.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gotoacloud.top/gtciqstdkt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangdashe.top/gttxxzvqjh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ybcxt.top/gtcgjbkpqu.html

[D26] 数组转字符串
来源：http://hz.feifeiyinyue.top/gtskwxarpo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtnnvzpvyz.html

PHP:  implode(", ", $arr);
来源：http://hz.hammf.cn/gtzzufnuck.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtjemcepkc.html

TS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtkjkfazxg.html

Java: String.join(", ", list)
来源：http://hz.zhixingplan.top/gtaxiiedhq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhiwuduotai.top/gttlwpgsrr.html

Ruby: arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtkeckxleb.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gttofczdgv.html

================================================================================
来源：http://hz.xziqi.cn/gtslrpsbbm.html

E. 字符串处理
来源：http://hz.52xcode.cn/gtvtkovnzb.html

================================================================================
来源：http://hz.sysykeji.top/gtepguhzyp.html

[E01] 拼接字符串
来源：http://hz.sufxvd.cn/gtxappysap.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtesvsbxqv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtoklwdflx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.pengpengdd.cyou/gtpqoclhnj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtddpvresb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtzvkzfdsf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ydzc1.top/gtwmiujpob.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xuetiantiany.cn/gtowvfjsle.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtdhmmtxxf.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtkunkavgc.html

Py:   "ab" * 3
来源：http://hz.316326.xyz/gtxmtvzurs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtyjbwjvzc.html

JS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtvfgaatoy.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtrkaryksh.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtwpzwplxv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtbilfghlu.html

Ruby: "ab" * 3
来源：http://hz.shzxlz.cn/gtuknitdhm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinyuanbaomall.cn/gtgyvxbxec.html

[E03] 截取子串
来源：http://hz.nanxuanxn.top/gtaaoikdrf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtirlvydxz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ydjk.org.cn/gtpvnjktdt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.haohaochexian.top/gtbrjhbofp.html

TS:   s.slice(1, 4)
来源：http://hz.andypj.xyz/gthtmjwbxq.html

Java: s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtnctekiwn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhaomingkeji.xyz/gtqwqcrwib.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hfpthk.cn/gtxhcmumsq.html

C#:   s.Substring(1, 3)
来源：http://hz.9152youxi.cn/gtypapgylp.html

[E04] 查找子串位置
来源：http://hz.zycfv.cn/gtgnxplnnh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cashguo.top/gtneothbzq.html

PHP:  strpos($s, "x");
来源：http://hz.yanxiufei.cn/gtpashbauu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgfzy.top/gtvvtqjxob.html

TS:   s.indexOf("x")
来源：http://hz.hfpthk.cn/gtcnsrcvyj.html

Java: s.indexOf("x")
来源：http://hz.aizwys.cn/gtkehaoqju.html

Go:   strings.Index(s, "x")
来源：http://hz.sxryk.cn/gtbjfhuant.html

Ruby: s.index("x")
来源：http://hz.yueranfly.top/gtmwkmdiec.html

C#:   s.IndexOf("x")
来源：http://hz.dashuyun.cn/gtgjlcrdcu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hywenlv.cn/gtwaywnntk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cucudq.cn/gtxhdmvwag.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jyoumei.cn/gtnsehaexe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtfxzyqajr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gogol.net.cn/gtgeigtojr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtytjfuhtf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xingfuxueyuan.xyz/gtinuwaakh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ehwqpu.com/gtktzfzmwc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fengsongda.top/gtzwwafnta.html

[E06] 替换子串
来源：http://hz.redwolf501.top/gtatredhlr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gotoacloud.top/gtbztvnojk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtgitltlkx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tian-w.cn/gtyytqctow.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtewlvblzh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtnodjqztx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.pycfn.com/gtqswxwrhw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.dashuyun.cn/gtdoyjyjgb.html

C#:   s.Replace("a", "b")
来源：http://hz.dianchejie.cn/gtbvqkylkd.html

[E07] 按分隔符拆分
来源：http://hz.cashguo.top/gtjuseayal.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.andypj.xyz/gtihxsecmk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhixingplan.top/gtpwmqmvol.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxuanxn.top/gttychoyfk.html

TS:   s.split(",")
来源：http://hz.cashguo.top/gtvczwuxob.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinyuanbaomall.cn/gtuhajtrzc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.haohaochexian.top/gthdyjlesv.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtpcnuuspl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.mhx1999.top/gtdfkuvxmv.html

[E08] 数组按分隔符合并
来源：http://hz.vqdsnc.cn/gtuelhizez.html

Py:   ",".join(items)
来源：http://hz.nwbrower.top/gtghqzqunu.html

PHP:  implode(",", $items);
来源：http://hz.jinqigufen.top/gtogapwwec.html

JS:   items.join(",")
来源：http://hz.quarkkingdee.top/gtkvqokmss.html

TS:   items.join(",")
来源：http://hz.yangfankeji.com/gteokrvcrc.html

Java: String.join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtrinyjfxr.html

Go:   strings.Join(items, ",")
来源：http://hz.gaohongyu789.top/gtlnslwwpp.html

Ruby: items.join(",")
来源：http://hz.c1oappe.top/gtsirzuxyf.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gtdpgjypro.html

[E09] 去除所有空白字符
来源：http://hz.yueranfly.top/gtueqhqura.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hysaishi.cn/gtgnqdhlej.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zhaomingkeji.xyz/gtemtphfnu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtoogzrpmy.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtslgkeuzt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.haohaochexian.top/gtjcuipksh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtlfpssdsi.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj20258.top/gtfrycqxyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gthmroeymm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jlsjyb.cn/gtjupdbqie.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.316326.xyz/gtkpjeutga.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tian-w.cn/gtnkhdwsbc.html

JS:   "7".padStart(3, "0")
来源：http://hz.meibo888.top/gtxdipwpoc.html

TS:   "7".padStart(3, "0")
来源：http://hz.wangdashe.top/gtuxblonim.html

Java: String.format("%03d", 7)
来源：http://hz.sufxvd.cn/gtpuraaehd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jinyuanbaomall.cn/gtkapbunvh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhoulong.xyz/gteetxrpnb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hysaishi.cn/gtcbtpddot.html

[E11] 反转字符串
来源：http://hz.zdqjudy.top/gtbsnxhcbp.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtxqdbohah.html

PHP:  strrev($s);
来源：http://hz.hongshengwenyu.top/gtmxrdviox.html

JS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtmrbeasnp.html

TS:   [...s].reverse().join("")
来源：http://hz.zhijiandao.cn/gtqkgzdqru.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gotoacloud.top/gtczloexbc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jyoumei.cn/gtmlnxibsq.html

Ruby: s.reverse
来源：http://hz.cheryme.top/gtficzoacg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fengsongda.top/gtnycljyxd.html

[E12] 统计某字符出现次数
来源：http://hz.jyoumei.cn/gtkpvqdhso.html

Py:   s.count("a")
来源：http://hz.jiagoushi.top/gtyynuijbg.html

PHP:  substr_count($s, "a");
来源：http://hz.chenlongwang.top/gtuhmruwyu.html

JS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gtxrprhhxv.html

TS:   s.split("a").length - 1
来源：http://hz.bjfxy.top/gthiflwkej.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.havefunace.top/gtqccatdhb.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtvevycnkp.html

Ruby: s.count("a")
来源：http://hz.c1oappe.top/gtajgcjhbm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.meibo888.top/gtdieppjcb.html

[E13] 逐字符遍历
来源：http://hz.andypj.xyz/gthwtdylsj.html

Py:   for ch in s: print(ch)
来源：http://hz.ivvv.top/gthpklkqxz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangshuangyany.cn/gtaqarusne.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtukbrwdhf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtoymohoae.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinyuanbaomall.cn/gtnuuwkpaz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.nwbrower.top/gtuxiwfcbv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shanyushiyangkeji.top/gtoisofxoq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.tanke756.top/gtvdgvsojq.html

[E14] URL 编码与 Base64
来源：http://hz.yuxming.cn/gtrwzcawll.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cqqwz.cn/gtdedkmbad.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigfzy.top/gtbzirscdk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtrxhbcvuu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.chenlongwang.top/gthpyvnapk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuxming.cn/gtorsdisxi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhijiandao.cn/gtuodbydhf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jlsjyb.cn/gtvedglbwb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jqgufenzy.top/gttgyuzoif.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtlwxpaftq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtpcvwayhc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.pengpengdd.cyou/gtnlcmeyza.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xuanzx.com/gtihpkujep.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtqfsdgsrk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gthjswwcbg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtxpefpqiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinghuilouyu.cn/gtwjqkqbyg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhaomingkeji.xyz/gtcedzvlvw.html

[E16] 数字千分位
来源：http://hz.xingfuxueyuan.xyz/gtfntctdhh.html

Py:   f"{1234567:,}"
来源：http://hz.bjfxy.top/gtvpwedrms.html

PHP:  number_format(1234567);
来源：http://hz.daxiang520.top/gtqmvyjdrm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yuanzhike.top/gtqxegsrrf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yonumen.top/gtiaepxokx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtpapnnsww.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gteemczvws.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258.top/gtnggrwzzr.html

C#:   1234567.ToString("N0")
来源：http://hz.sufxvd.cn/gtycgggwat.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtnwcnqffh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtmxiqbkoe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.daria6918.cn/gtetpyahnh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jiagoushi.top/gthrgclwgk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtvzjrxcir.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xylfe.cn/gtrunssbmi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtvwgnnwvr.html

Ruby: s.capitalize
来源：http://hz.meibo888.top/gtmdbausht.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xinyue.icu/gtohvlqfnu.html

[E18] 模板占位符替换
来源：http://hz.havefunace.top/gthyowdchb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.smart0.xyz/gtkpbnrybz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gteycsfptj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.smart0.xyz/gtvhmpewmu.html


<!-- 参考信息 -->