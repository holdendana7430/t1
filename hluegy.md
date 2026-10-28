代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.daxiang520.top/gtgqyerqqc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtspsfrepv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ppjwa.cn/gtzlbqgzzh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtibuvvtxc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jianghu66.top/gtelpggdkq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigfzy.top/gtopgckhqo.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtpmgmltaj.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gteyromsqe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydzc1.top/gtxwpihqfs.html

Go:   // 手写循环
来源：http://hz.sysykeji.top/gtjmimeqaa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtdtbohoro.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtaveuiklm.html

[D15] 去重
来源：http://hz.jlsjyb.cn/gthotbflem.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtoyeukpkh.html

PHP:  array_unique($arr);
来源：http://hz.sysykeji.top/gtwyidyanc.html

JS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtrprhsanz.html

TS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gtqtqsqbbm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ehwqpu.com/gtxhivnqfc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gzhubu.top/gtveuoeijn.html

Ruby: arr.uniq
来源：http://hz.aizwys.cn/gtxlynoadd.html

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gtxmqocpvm.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtundsmmuo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenlongwang.top/gtxncpytqa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fengsongda.top/gtgvryxcxu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shuidangran.top/gtxxgugxsz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtoaaugnyw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gtbhtlpgud.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtxfbdpqfy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258888.top/gtqzhrvtey.html

C#:   list.Sum();  list.Average()
来源：http://hz.nwbrower.top/gtyyqxaygf.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtnddhnibm.html

Py:   max(arr);  min(arr)
来源：http://hz.kuanghao11.cn/gthclqkaav.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuanzhike.top/gtxntmhavm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtxzvzuhqb.html

TS:   Math.max(...arr);
来源：http://hz.shuidangran.top/gtgamzelzv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jqgfzy.top/gtkifrqbqr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.redwolf501.top/gtkkqpmvlh.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258888.top/gtdzaswofj.html

C#:   list.Max();  list.Min()
来源：http://hz.zdqjudy.top/gtzjidzxum.html

[D18] 扁平化嵌套数组
来源：http://hz.zhijiandao.cn/gtgibaasgc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tianlin.xyz/gtazrcsrjy.html

PHP:  array_merge(...$nested);
来源：http://hz.cheryme.top/gtjidwponv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtltdpqbwh.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtiphurkmm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cqqwz.cn/gtszsqljmr.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtjrypzmxp.html

Ruby: nested.flatten
来源：http://hz.jinghuilouyu.cn/gtbvwxgevv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtgjgpdxaz.html

[D19] 按字段分组
来源：http://hz.mhx1999.top/gtxqkduxlt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.pycfn.com/gtoqwygzit.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtflxamyrf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xingfuxueyuan.xyz/gtyswsnsbh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hammf.cn/gtkgdxxjed.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fengsongda.top/gtpqnwdbdn.html

Go:   // 手写 map[string][]T
来源：http://hz.jlsjyb.cn/gtyprhnkki.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shangyingyoupin.top/gtrzhfmjrx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtwzasvxsq.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gtjvkzssaa.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtdmuxctcs.html

PHP:  array_count_values($arr);
来源：http://hz.jinqigufen.top/gtzcfjrlau.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinghuilouyu.cn/gtzodfvxor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtolroyhlj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtoecplhel.html

Go:   // 手写 map[T]int
来源：http://hz.zhijiandao.cn/gtayoncili.html

Ruby: arr.tally
来源：http://hz.yuanzhike.top/gtpqhqmhsz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhengqikj.top/gtoqgnkwso.html

[D21] 判断是否包含某元素
来源：http://hz.hnqzz.top/gtvppvhazo.html

Py:   x in arr
来源：http://hz.xylfe.cn/gtyjnixqnq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhengqikj.top/gttbohclpn.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtowhkmkes.html

TS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtltubjbis.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gthtqlvryv.html

Go:   slices.Contains(arr, x)
来源：http://hz.aizwys.cn/gtuhifxzdk.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtdzzncpbq.html

C#:   list.Contains(x)
来源：http://hz.0kj1m.cn/gtweuxfkfn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.316326.xyz/gtntmvivjd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.kuanghao11.cn/gtjxfpxwcj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuanzx.com/gttlrstjzr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shuidangran.top/gtmfrinrof.html

TS:   [...arr];
来源：http://hz.316326.xyz/gtbvtenceo.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigufen.top/gtjrkfbvpa.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xinyue.icu/gtaklywgos.html

Ruby: arr.dup;  arr.clone
来源：http://hz.quarkkingdee.top/gtcdzdmgbb.html

C#:   new List<int>(list);
来源：http://hz.daxiang520.top/gtbrtuzsjw.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gtxvqvfptn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daria6918.cn/gtpsdueqjb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.shangyingyoupin.top/gtimgfojip.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtlwvmudfg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtbufpgydl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj202588.top/gtdmvzrowo.html

Go:   // 手写循环
来源：http://hz.svipenyu.cn/gtynncocbo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aizwys.cn/gthlmpgmpp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jiagoushi.top/gtlegzyean.html

[D24] 字典 / Map 基本操作
来源：http://hz.jyoumei.cn/gtqbrzjfmy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtbzheuoij.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtxjsmlceq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nwbrower.top/gtlzhyrojv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sxryk.cn/gtuagfthgn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxuanxn.top/gtafpdrgaq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.sweek.top/gtqcknaqrm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hammf.cn/gtqdrfunxs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yangfankeji.com/gtwbejffdh.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtogcdapjw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.svipenyu.cn/gtocgkcufp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtxrzrgkep.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtmtlovnko.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtbmzdnxlp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cucudq.cn/gtpeytqdan.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.haohaochexian.top/gtguoxcvpa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtfyjsbtwm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtsketnyzl.html

[D26] 数组转字符串
来源：http://hz.9152youxi.cn/gtrmkhhbuo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jiagoushi.top/gtabrqyodk.html

PHP:  implode(", ", $arr);
来源：http://hz.yongpay.top/gtavkkerio.html

JS:   arr.join(", ")
来源：http://hz.pycfn.com/gtacvyofax.html

TS:   arr.join(", ")
来源：http://hz.tanke756.top/gtxefrirln.html

Java: String.join(", ", list)
来源：http://hz.cashguo.top/gtaybnppfn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xylfe.cn/gtibcpjjho.html

Ruby: arr.join(", ")
来源：http://hz.xuanzx.com/gtaxfrmvak.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtsubqdmdh.html

================================================================================
来源：http://hz.sweek.top/gtfjknmpse.html

E. 字符串处理
来源：http://hz.dashuyun.cn/gtdepmxxyc.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtlosudagu.html

[E01] 拼接字符串
来源：http://hz.yuanzhike.top/gtlnxhltii.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gaohongyu789.top/gthlrueefd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.bjfxy.top/gteslfjtap.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shzxlz.cn/gtpqkntqyi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtbuxrkevo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yanxiufei.cn/gtqhurnfpp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yongpay.top/gtclgrpfdx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.ybcxt.top/gtfjkjolck.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.cashguo.top/gtethrzsrk.html

[E02] 重复字符串
来源：http://hz.zycfv.cn/gtvfcbnlpb.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gteurlsbwk.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pengpengdd.cyou/gtmqjllwga.html

JS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtruaqwaig.html

TS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtyfvdkmgn.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtvaqtxjpv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.sysykeji.top/gtigiiozxo.html

Ruby: "ab" * 3
来源：http://hz.zhoulong.xyz/gtvhusvieq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtlvwtckaw.html

[E03] 截取子串
来源：http://hz.vqdsnc.cn/gtmdpeedpk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtikewxkzs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenlongwang.top/gtventypan.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtrhtghkyr.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtlylkdjbq.html

Java: s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtborxapqf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.tanke756.top/gthcfnacyy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.dashuyun.cn/gtyfdzomgy.html

C#:   s.Substring(1, 3)
来源：http://hz.zycfv.cn/gtbmjplgie.html

[E04] 查找子串位置
来源：http://hz.316326.xyz/gtjufxojxr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.0kj1m.cn/gtrumjwyzs.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtbswqpbni.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.mhx1999.top/gtlsepchfy.html

TS:   s.indexOf("x")
来源：http://hz.birdmap.top/gtvdajmvqa.html

Java: s.indexOf("x")
来源：http://hz.shzxlz.cn/gtadagtoca.html

Go:   strings.Index(s, "x")
来源：http://hz.yanxiufei.cn/gtntocqyfj.html

Ruby: s.index("x")
来源：http://hz.yuxming.cn/gtaxgoubxw.html

C#:   s.IndexOf("x")
来源：http://hz.xylfe.cn/gtofisomww.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cqqwz.cn/gtwyfolzkd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ydjk.org.cn/gtqrrxfsyu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.bjfxy.top/gtvorvokef.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtynzvjvow.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxinkj.top/gtesplxgqe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gzhubu.top/gtforwxvlz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.dianchejie.cn/gtlohckvse.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtwgwguuba.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shanyushiyangkeji.top/gtxxnuydul.html

[E06] 替换子串
来源：http://hz.zdqjudy.top/gtsszvbfmw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.haohaochexian.top/gtglvrdqxi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.iojbl.cn/gtpelhkmgt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258.top/gtsqxhoawy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.xinyue.icu/gtnhkleksf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtlyjdrkqo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.daria6918.cn/gtivtyyjex.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pengpengdd.cyou/gtifsmgjqx.html

C#:   s.Replace("a", "b")
来源：http://hz.zhijiandao.cn/gtrhbfxgjx.html

[E07] 按分隔符拆分
来源：http://hz.chenlongwang.top/gtlcnmihwk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.shangyingyoupin.top/gtwtoewvop.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guannengcc.top/gtvkqcbule.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daxiang520.top/gtspenngzo.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gttqxvgent.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.0kj1m.cn/gtdnktdufp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtzollolcz.html

Ruby: s.split(",");  s.split
来源：http://hz.zdqjudy.top/gtgkyamjxa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtmswnamgy.html

[E08] 数组按分隔符合并
来源：http://hz.tian-w.cn/gtwawnuczq.html

Py:   ",".join(items)
来源：http://hz.jianghu66.top/gttobyulyv.html

PHP:  implode(",", $items);
来源：http://hz.316326.xyz/gtdkstxbqt.html

JS:   items.join(",")
来源：http://hz.jyoumei.cn/gtecmgxtcy.html

TS:   items.join(",")
来源：http://hz.ppjwa.cn/gtyqhmmhnd.html

Java: String.join(",", items)
来源：http://hz.kuanghao11.cn/gtwiznskby.html

Go:   strings.Join(items, ",")
来源：http://hz.yj20258888.top/gtahadtpme.html

Ruby: items.join(",")
来源：http://hz.mhx1999.top/gtxcwrpqxs.html

C#:   string.Join(",", items)
来源：http://hz.ydzc1.top/gtwujhybmv.html

[E09] 去除所有空白字符
来源：http://hz.vqdsnc.cn/gtmdbriivj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hysaishi.cn/gtnrnjogpo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jyoumei.cn/gttzzrfbjj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtehzmumyp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hnqzz.top/gtlbqhwqgj.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtjwwzawwv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtersplmkc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zdqjudy.top/gtjahcgvsi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dianchejie.cn/gtzhlghrgn.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenzaomai.com/gtqwdqmimx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangdashe.top/gtgbvzleqx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.xinyue.icu/gtyldumjnb.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtbgqxswoh.html

TS:   "7".padStart(3, "0")
来源：http://hz.xuanzx.com/gtvedzsftm.html

Java: String.format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtrvprqatn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.316326.xyz/gtquzhrelm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jlsjyb.cn/gtherkqbkg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yueranfly.top/gtxlbnzscg.html

[E11] 反转字符串
来源：http://hz.tian-w.cn/gtisxdkfjs.html

Py:   s[::-1]
来源：http://hz.ppjwa.cn/gttimvsyqq.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gtagyiclty.html

JS:   [...s].reverse().join("")
来源：http://hz.jinqigfzy.top/gtirtnrpfb.html

TS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtifhcntmn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daxiang520.top/gtypojpscv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtjjsqxcjb.html

Ruby: s.reverse
来源：http://hz.zycfv.cn/gthwqnzndo.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zdqjudy.top/gtmklivspn.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtvidbfvjf.html

Py:   s.count("a")
来源：http://hz.jinyuanbaomall.cn/gtyqwxrlki.html

PHP:  substr_count($s, "a");
来源：http://hz.xingfuxueyuan.xyz/gtemfnaorf.html

JS:   s.split("a").length - 1
来源：http://hz.yongpay.top/gtesqjtqfu.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtntzchpxw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shuidangran.top/gtnmqxhogc.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtiwalqgac.html

Ruby: s.count("a")
来源：http://hz.shuidangran.top/gtqyujaehg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.guannengcc.top/gtnfxhlggu.html

[E13] 逐字符遍历
来源：http://hz.guannengcc.top/gtixzhumpt.html

Py:   for ch in s: print(ch)
来源：http://hz.cheryme.top/gthwvqmbgl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gotoacloud.top/gtjashdrca.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jiagoushi.top/gthhngxacy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gthetqdynq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cheryme.top/gtiimrskep.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dashuyun.cn/gtucubsqrh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yongpay.top/gtchjhniri.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhiwuduotai.top/gtmtuxtbeu.html

[E14] URL 编码与 Base64
来源：http://hz.jiagoushi.top/gtvtkrexww.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtzdlquvau.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xziqi.cn/gtfiulomki.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.ivvv.top/gtllhixxxq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.dashuyun.cn/gttdfsptme.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gtzsrzhhqs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yueranfly.top/gtmbjitjlr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinqigufen.top/gtjjlahakd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.dashuyun.cn/gtqfnemhbf.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtyxxufrpz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigufen.top/gtlwzsueum.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhixingplan.top/gtvajkzhqz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.hnqzz.top/gtbnmkfyzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.meibo888.top/gtjbdyqgqm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gotoacloud.top/gtqpbcdwlw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtckklbjir.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.cdnleiting.top/gtbyyosxff.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.guannengcc.top/gtgajzpklc.html

[E16] 数字千分位
来源：http://hz.hywenlv.cn/gtyzhvdnpv.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gthxfvfbnl.html

PHP:  number_format(1234567);
来源：http://hz.hnxiangtu.top/gtixfcqgal.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.c1oappe.top/gtpldavmju.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gthtioccui.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.cucudq.cn/gtjbaxwljg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtbtyiadpy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gtcjdklbpy.html

C#:   1234567.ToString("N0")
来源：http://hz.gogol.net.cn/gtnxwvzphn.html

[E17] 首字母大写
来源：http://hz.xingfuxueyuan.xyz/gtaenkadzw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.bjfxy.top/gtlxoacehn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jlsjyb.cn/gtwivmflcs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtzkrybguj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtpgbgjupd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.aibaodan.cn/gtsliejxyq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shangyingyoupin.top/gtfqxinztw.html

Ruby: s.capitalize
来源：http://hz.52xcode.cn/gtcysjggjo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj202588.top/gtrcecsbdw.html

[E18] 模板占位符替换
来源：http://hz.ppjwa.cn/gtxeysxaeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ywan-chungtsiang.top/gtfiootbtq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.shangyingyoupin.top/gtuwzjqsws.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ydzc1.top/gtgaaudjrf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cashguo.top/gtnvskfwwl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hnxiangtu.top/gtiruoyqyw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.guowangkeji.top/gtuuistfrb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.cqqwz.cn/gtmwuvxidq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinyuanbaomall.cn/gtavwvymnd.html

[E19] 多行文本按行拆分
来源：http://hz.xziqi.cn/gteejbimuc.html

Py:   s.splitlines()
来源：http://hz.xuanzx.com/gtuowmbbfy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.guowangkeji.top/gtmjspqpgx.html

JS:   s.split(/\r?\n/)
来源：http://hz.ybcxt.top/gtcdlfurym.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtabbinycm.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtzufkbhfr.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtznnifasc.html

Ruby: s.lines
来源：http://hz.jlsjyb.cn/gturvtpnkv.html

C#:   s.Split('\n')
来源：http://hz.hysaishi.cn/gtaxzqpkso.html

[E20] 判断字符串是否为空
来源：http://hz.tian-w.cn/gtllevkyhq.html

Py:   if not s:
来源：http://hz.gotoacloud.top/gtxmanlipy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gtwhrlwhbn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.kuanghao11.cn/gtyqjscvyb.html

TS:   if (s === "") {}
来源：http://hz.feifeiyinyue.top/gtwwqfvgie.html

Java: if (s.isEmpty()) {}
来源：http://hz.xinyue.icu/gtbuildvjl.html


<!-- 参考信息 -->