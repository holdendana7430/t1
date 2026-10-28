代发 wailian999

C#:   list.Reverse();
来源：http://hz.shanyushiyangtech.top/gtopnmsmwc.html

[D12] 查找元素下标
来源：http://hz.chenlongwang.top/gtwttxgkvi.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhaomingkeji.xyz/gtvxwroxar.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinyuanbaomall.cn/gtjxptyojt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtphzuaklq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtqbwspbwy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtsgkzycja.html

Go:   slices.Index(arr, x)
来源：http://hz.iojbl.cn/gtogmtdddc.html

Ruby: arr.index(x)
来源：http://hz.sweek.top/gtrcozmloh.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtedczpvkb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yvedp.cn/gtyfvggobo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtgljzejjz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtxuxejokq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenlongwang.top/gtwqnoticz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtmpoenbog.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cqqwz.cn/gtcvhijyqe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.svipenyu.cn/gtlnocwmcb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aibaodan.cn/gtzlbwqweg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.52xcode.cn/gtcdvfyvoz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shangyingyoupin.top/gtetnjveit.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj202588.top/gteclkriut.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtyeigpqse.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtenkdxozm.html

TS:   arr.map(x => x * 2)
来源：http://hz.yvedp.cn/gtktsbscqw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gtvdfmfqsp.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtrxodheud.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shangyingyoupin.top/gtjqbedodr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hfpthk.cn/gtoyatwufn.html

[D15] 去重
来源：http://hz.iojbl.cn/gtglrxcmbt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xziqi.cn/gtngtkxoju.html

PHP:  array_unique($arr);
来源：http://hz.ehwqpu.com/gtwzgfzuxo.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtxqpayosk.html

TS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtvdqikfjx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.meibo888.top/gtqulbtzvx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ivvv.top/gtwmbqcsjr.html

Ruby: arr.uniq
来源：http://hz.9152youxi.cn/gtbsvqhgzd.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gtonyubrua.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtolvxfbfo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.iojbl.cn/gtagbxbbpt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtxpljaaom.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtrzbcmebu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtsnbsvrbl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.kuanghao11.cn/gttxjnefyh.html

Go:   // 手写循环累加
来源：http://hz.9152youxi.cn/gtoanhxnmu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gtpknhhihn.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxinkj.top/gtqkbrwbcs.html

[D17] 最大值与最小值
来源：http://hz.0kj1m.cn/gtfbyfwpcm.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtbpkuztpe.html

PHP:  max($arr);  min($arr);
来源：http://hz.sysykeji.top/gteoqfzzqi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtlvvjilxp.html

TS:   Math.max(...arr);
来源：http://hz.bjfxy.top/gtgftepssh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtnwhaoidz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gtrzduhujc.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigfzy.top/gtbvjxsoxx.html

C#:   list.Max();  list.Min()
来源：http://hz.meibo888.top/gtcgvkwway.html

[D18] 扁平化嵌套数组
来源：http://hz.jlsjyb.cn/gtcnzjokpg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtkoviyghc.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258888.top/gtrvnsjnvu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shangyingyoupin.top/gtdmnychsw.html

TS:   nested.flat();
来源：http://hz.jqgfzy.top/gtgihlmtql.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtzpuhqbjy.html

Go:   // 手写双层循环
来源：http://hz.birdmap.top/gtuzkgedil.html

Ruby: nested.flatten
来源：http://hz.zhoulong.xyz/gteoculwvw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtydxnfoow.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtaaaazkwa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtlkdazngv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sweek.top/gtiujfhoci.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydjk.org.cn/gtxxtzwjku.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gttnzicqvd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gaohongyu789.top/gtsulixbxb.html

Go:   // 手写 map[string][]T
来源：http://hz.cdnleiting.top/gtrmlbpwwm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gtshuxujye.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shuidangran.top/gthkjjnctl.html

[D20] 统计每个元素出现次数
来源：http://hz.0kj1m.cn/gtbujylgnf.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gtgpcrctiy.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtcatkwxiw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gthzwhcofi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtevajjsli.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenjidiqi.icu/gtfzjedyft.html

Go:   // 手写 map[T]int
来源：http://hz.feifeiyinyue.top/gtemdavbqb.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtalujprgz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.fengsongda.top/gtwgrachhj.html

[D21] 判断是否包含某元素
来源：http://hz.yvedp.cn/gtxtvcncsn.html

Py:   x in arr
来源：http://hz.iojbl.cn/gtpdhqlvji.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hnqzz.top/gtfhrdykwz.html

JS:   arr.includes(x)
来源：http://hz.sweek.top/gtjprkibey.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtujvkysbn.html

Java: list.contains(x)
来源：http://hz.nwbrower.top/gtxupdfxwd.html

Go:   slices.Contains(arr, x)
来源：http://hz.shzxlz.cn/gtalicgbcq.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtjauekhxn.html

C#:   list.Contains(x)
来源：http://hz.hnxiangtu.top/gtfwrahgxm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hysaishi.cn/gtnwtvvxkt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jlsjyb.cn/gtejmdlkon.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinyuanbaomall.cn/gtoclrwkij.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.redwolf501.top/gtxicvqrdf.html

TS:   [...arr];
来源：http://hz.ybcxt.top/gtxlroitvf.html

Java: new ArrayList<>(list);
来源：http://hz.yonumen.top/gtbpdjancl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jianghu66.top/gtzkehvvvl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tianlin.xyz/gtgxnbxbdb.html

C#:   new List<int>(list);
来源：http://hz.xinyue.icu/gtepwtjosn.html

[D23] reduce 累积计算
来源：http://hz.iojbl.cn/gtheiumgye.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangdashe.top/gtbanwfrms.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtzygnchff.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtjlwhgxxa.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.havefunace.top/gtgxkrzcgf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtoqwyhppx.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gteisshsya.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xuanzx.com/gtrmdvqhqp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hnqzz.top/gtiqmtzywh.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigufen.top/gtokgbfzbr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtbrkurkpg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtbnyozdgw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yangfankeji.com/gtelylqaif.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sxryk.cn/gtaxmvsmgd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shangyingyoupin.top/gtvrslxozy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuetiantiany.cn/gtevgihrun.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.316326.xyz/gtveqhileh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gzhubu.top/gtdcxvhgzm.html

[D25] Set 集合去重与交并差
来源：http://hz.pengpengdd.cyou/gtmdpibwuu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gtqqcmolzp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xinyue.icu/gttvxfsots.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gtunpotgaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtjywqszkl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daxiang520.top/gtpxqeidvk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.iojbl.cn/gtrmzvottq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.aizwys.cn/gthvesknfn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigfzy.top/gtnlwdhepm.html

[D26] 数组转字符串
来源：http://hz.xuetiantiany.cn/gtiwpyejwa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shangyingyoupin.top/gtofidizfy.html

PHP:  implode(", ", $arr);
来源：http://hz.yonumen.top/gtrnkugblj.html

JS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtgvnlnkij.html

TS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtesnumung.html

Java: String.join(", ", list)
来源：http://hz.yuanzhike.top/gtciernekh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hammf.cn/gtcytcwekz.html

Ruby: arr.join(", ")
来源：http://hz.yj202588.top/gtwchcivwj.html

C#:   string.Join(", ", list)
来源：http://hz.tian-w.cn/gtyymoetcp.html

================================================================================
来源：http://hz.wangdashe.top/gtxvohwdoe.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtquklnmut.html

================================================================================
来源：http://hz.meibo888.top/gteezitifj.html

[E01] 拼接字符串
来源：http://hz.svipenyu.cn/gtazerbymo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigufen.top/gtowcspoer.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtcgiukbeh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gtamtbpmms.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtskrpromm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.52xcode.cn/gteznydaph.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.pengpengdd.cyou/gteblvofqr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhiwuduotai.top/gtaczujfag.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hysaishi.cn/gtmctytgug.html

[E02] 重复字符串
来源：http://hz.gzhubu.top/gtybovcibh.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtptwgpsuv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.0kj1m.cn/gtjrgwhotp.html

JS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtedvxrxvl.html

TS:   "ab".repeat(3)
来源：http://hz.cqqwz.cn/gtwjgfgijn.html

Java: "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtvqcsybka.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nwbrower.top/gtbeogphbd.html

Ruby: "ab" * 3
来源：http://hz.gaohongyu789.top/gtqpdgqzph.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hnxiangtu.top/gtvtzukqcr.html

[E03] 截取子串
来源：http://hz.chenlongwang.top/gtznisguax.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gogol.net.cn/gtjusudzcc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuanzx.com/gtestgybvt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtgqwfzkes.html

TS:   s.slice(1, 4)
来源：http://hz.fzhhl.top/gtvuzsfwuw.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gtjnsemenb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guowangkeji.top/gtxfncxukz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.cashguo.top/gtqzhtqweg.html

C#:   s.Substring(1, 3)
来源：http://hz.yongpay.top/gtxhudkspr.html

[E04] 查找子串位置
来源：http://hz.yuxming.cn/gtcpmbbwrh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangtech.top/gtwtpxqqxl.html

PHP:  strpos($s, "x");
来源：http://hz.hnqzz.top/gtvlgdhrsp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.cucudq.cn/gttkpmgdey.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gttgmmqwqp.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gtqikathtf.html

Go:   strings.Index(s, "x")
来源：http://hz.redwolf501.top/gtaucfgaee.html

Ruby: s.index("x")
来源：http://hz.dashuyun.cn/gtnqydnxcn.html

C#:   s.IndexOf("x")
来源：http://hz.52xcode.cn/gtaidjkwua.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sweek.top/gttqgwsvio.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtoensrltt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guowangkeji.top/gtyzbeqnuy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jlsjyb.cn/gtynbikved.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zycfv.cn/gtsxrifmtl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.quarkkingdee.top/gtfnxcmcul.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gaohongyu789.top/gtwfmovhbw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinyuanbaomall.cn/gtflmbjudg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fzhhl.top/gtaonbntlm.html

[E06] 替换子串
来源：http://hz.kuanghao11.cn/gtdnldcwjv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xziqi.cn/gtordbtdzz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sufxvd.cn/gttlmzqjck.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtufyrpaxm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhijiandao.cn/gtfttlkfpu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtcrrgpfff.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.hfpthk.cn/gtydmcnqnr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtcvmudjrv.html

C#:   s.Replace("a", "b")
来源：http://hz.jlsjyb.cn/gtjcnnazla.html

[E07] 按分隔符拆分
来源：http://hz.xinyue.icu/gtsgptqatt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.havefunace.top/gtilosujtq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yongpay.top/gtyqbfmnns.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuetiantiany.cn/gtvheetqxq.html

TS:   s.split(",")
来源：http://hz.xylfe.cn/gtnkkjsiel.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtwadglkye.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ywan-chungtsiang.top/gtuvcuoddx.html

Ruby: s.split(",");  s.split
来源：http://hz.zhoulong.xyz/gtoxgaorfb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxinkj.top/gtrsydfmzx.html

[E08] 数组按分隔符合并
来源：http://hz.xingfuxueyuan.xyz/gtfvpxuafw.html

Py:   ",".join(items)
来源：http://hz.pengpengdd.cyou/gtpcyfskcz.html

PHP:  implode(",", $items);
来源：http://hz.hnxiangtu.top/gtoabzxwdv.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtjkxirgat.html

TS:   items.join(",")
来源：http://hz.fzhhl.top/gteoogadsx.html

Java: String.join(",", items)
来源：http://hz.yangfankeji.com/gtxokpprdc.html

Go:   strings.Join(items, ",")
来源：http://hz.zhoulong.xyz/gtzfagyxgo.html

Ruby: items.join(",")
来源：http://hz.tian-w.cn/gtdbzghbwj.html

C#:   string.Join(",", items)
来源：http://hz.ydjk.org.cn/gttfdemael.html

[E09] 去除所有空白字符
来源：http://hz.daria6918.cn/gtcnvtegcs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gogol.net.cn/gtqeskkrye.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangdashe.top/gtnxeeipjl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtyxlbqpkl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtukqiiqpk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnxiangtu.top/gtdayujcjr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.birdmap.top/gtgstyktrr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jlsjyb.cn/gtcmnienvt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.52xcode.cn/gtzodhcjaq.html

[E10] 左侧补零 / 定长填充
来源：http://hz.tanke756.top/gtrmuoinwf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtqrdutrni.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.birdmap.top/gtoudndlty.html

JS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gteoonndjh.html

TS:   "7".padStart(3, "0")
来源：http://hz.guowangkeji.top/gtzcdzsije.html

Java: String.format("%03d", 7)
来源：http://hz.hysaishi.cn/gtrvecinvg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xinyue.icu/gtlwscziee.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtzhqmdrbl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sysykeji.top/gttnfvdixo.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gtwmyrrjsb.html

Py:   s[::-1]
来源：http://hz.bjfxy.top/gtmdhxkhjk.html

PHP:  strrev($s);
来源：http://hz.jqgfzy.top/gtakxomjwm.html

JS:   [...s].reverse().join("")
来源：http://hz.feifeiyinyue.top/gtomrwbyaq.html

TS:   [...s].reverse().join("")
来源：http://hz.zdqjudy.top/gtsxgznaij.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yvedp.cn/gtozmxeuhr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.0kj1m.cn/gtlaififfv.html

Ruby: s.reverse
来源：http://hz.cucudq.cn/gthvekaaje.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtsjmuweoh.html

[E12] 统计某字符出现次数
来源：http://hz.xziqi.cn/gtckleocow.html

Py:   s.count("a")
来源：http://hz.yvedp.cn/gtpcmcgfoq.html

PHP:  substr_count($s, "a");
来源：http://hz.guannengcc.top/gtdywiwqqa.html

JS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtoqzjkntl.html

TS:   s.split("a").length - 1
来源：http://hz.zhaomingkeji.xyz/gtmfmcaoqr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nwbrower.top/gtigbpgdtv.html

Go:   strings.Count(s, "a")
来源：http://hz.yj20258.top/gtckaunfuv.html

Ruby: s.count("a")
来源：http://hz.cheryme.top/gtoqvlylck.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gogol.net.cn/gtzomkdest.html

[E13] 逐字符遍历
来源：http://hz.yuxming.cn/gtohvntlrm.html

Py:   for ch in s: print(ch)
来源：http://hz.c1oappe.top/gtbsmjgihh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yj20258888.top/gtflfwpeyb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jianghu66.top/gtarrdabcp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangdashe.top/gtjzbafwlu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ybcxt.top/gtxasnorwe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.dianchejie.cn/gtdiwjfeuz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jqgufenzy.top/gtdjbtxbnm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yueranfly.top/gtbjatyuej.html

[E14] URL 编码与 Base64
来源：http://hz.haohaochexian.top/gtsbnqmwqi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgufenzy.top/gtaqbimjka.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cheryme.top/gtfkuzfari.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtdqioslyy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sweek.top/gtdmxqbbtw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.0kj1m.cn/gtabkvzhxd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gogol.net.cn/gtbeznrvaf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtsgpsbyss.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yj20258.top/gtndmgviaw.html

[E15] HTML 转义 / 反转义
来源：http://hz.ywan-chungtsiang.top/gtpugenxmz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtlfnagcbu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yj20258888.top/gtrqruikvx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.fzhhl.top/gtdmjqpfpm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.meibo888.top/gtvhtyxqoy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cqqwz.cn/gtwidteiur.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gzhubu.top/gtebetkqtx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.nanxuanxn.top/gtircapfnp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtjeymwbcn.html

[E16] 数字千分位
来源：http://hz.yanxiufei.cn/gtvyhdcyax.html

Py:   f"{1234567:,}"
来源：http://hz.guannengcc.top/gtnxwwslcy.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gtumaakoce.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtdrtpztzp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.havefunace.top/gtsrcwcjdg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.mhx1999.top/gtpffdauqc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hnxiangtu.top/gtbmwufbvm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jinghuilouyu.cn/gtpbbyzpip.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtxscwqhqm.html

[E17] 首字母大写
来源：http://hz.ybcxt.top/gtulcdksjq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.kuanghao11.cn/gtgnfkqlkr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yj20258888.top/gtznkmcacr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtlnexhkxy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.guannengcc.top/gtybeybxqs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gttjghydox.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yuanzhike.top/gtbfsdkkjw.html

Ruby: s.capitalize
来源：http://hz.guannengcc.top/gtqjnpthko.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hywenlv.cn/gtkuifahqp.html

[E18] 模板占位符替换
来源：http://hz.hnxiangtu.top/gtrvjatjei.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cashguo.top/gtvmxbmxqv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtslpmxvdo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gtaadbjjwp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxinkj.top/gtrstssrip.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.c1oappe.top/gtpyojxyzl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.bjfxy.top/gtqlqydjxq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.52xcode.cn/gtcmtnzlzl.html


<!-- 参考信息 -->