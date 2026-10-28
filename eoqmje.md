代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtlgxwmqzs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtvfgmlluw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gtrambuuxx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hongshengwenyu.top/gttdeyoohw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtbemggqzn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangkeji.top/gtzskyvyix.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtvjzcadkp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daxiang520.top/gtrtruucwh.html

[D11] 反转数组
来源：http://hz.smart0.xyz/gtrqimwpgr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinghuilouyu.cn/gtvpafevmi.html

PHP:  array_reverse($arr);
来源：http://hz.pycfn.com/gtoskzfeag.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinghuilouyu.cn/gteaetnvqn.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtzlozwaic.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gttdliybzu.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtmwnutamr.html

Ruby: arr.reverse
来源：http://hz.dianchejie.cn/gtkkbtjtmw.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtjssacgzs.html

[D12] 查找元素下标
来源：http://hz.gzhubu.top/gttvmkrwpe.html

Py:   arr.index(x);  x in arr
来源：http://hz.redwolf501.top/gtuykblrkd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhijiandao.cn/gteqrphpsc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtaindfyga.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtdzrkkyml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtqbdompwq.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gtjqcojgsh.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtnfwhafnq.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtodmswxzv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shangyingyoupin.top/gtjsajzmmi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.pengpengdd.cyou/gtunlbgstu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ywan-chungtsiang.top/gtwpxsfeil.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sysykeji.top/gtptnxvhbx.html

TS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtjmfpkmej.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shzxlz.cn/gtwwozghem.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangshuangyany.cn/gtcdnspaly.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtjvsbyrvr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dianchejie.cn/gtxkdqoyzo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtxxydksdj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.zhijiandao.cn/gtefougfzj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shzxlz.cn/gtmaetemek.html

JS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtdlxgenxs.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtucapapln.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtsreclhbn.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtncecztqe.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hysaishi.cn/gtgaoxocyj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtyzvqrnav.html

[D15] 去重
来源：http://hz.hysaishi.cn/gtacqargjz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.sufxvd.cn/gtgeahcxau.html

PHP:  array_unique($arr);
来源：http://hz.hnxiangtu.top/gtqdelfcfq.html

JS:   [...new Set(arr)]
来源：http://hz.tian-w.cn/gtsjtbreqk.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtckfycmiz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.feifeiyinyue.top/gtzwnykghm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangkeji.top/gtmrwtdorh.html

Ruby: arr.uniq
来源：http://hz.shanyushiyangkeji.top/gtdsvftmaj.html

C#:   list.Distinct().ToList()
来源：http://hz.aibaodan.cn/gtvvuqgrib.html

[D16] 求和与平均值
来源：http://hz.yj20258.top/gtjwphjrgv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangshuangyany.cn/gtdnuzcssn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtxfsfnmvn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtdxbuuepp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xinyue.icu/gtfqilwfgd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.redwolf501.top/gttcdcjbiy.html

Go:   // 手写循环累加
来源：http://hz.xuetiantiany.cn/gtnwbvrxbr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gotoacloud.top/gtlfjtmpmc.html

C#:   list.Sum();  list.Average()
来源：http://hz.sxryk.cn/gtwarqfiwc.html

[D17] 最大值与最小值
来源：http://hz.vqdsnc.cn/gtxzabqhlq.html

Py:   max(arr);  min(arr)
来源：http://hz.jqgufenzy.top/gtauzuptgo.html

PHP:  max($arr);  min($arr);
来源：http://hz.iojbl.cn/gtsqkvnpgh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cdnleiting.top/gtmhqyliex.html

TS:   Math.max(...arr);
来源：http://hz.zycfv.cn/gtexjmejlc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gthdwmbenp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnqzz.top/gtjaherknq.html

Ruby: arr.max;  arr.min
来源：http://hz.cucudq.cn/gtibhzmoel.html

C#:   list.Max();  list.Min()
来源：http://hz.xingfuxueyuan.xyz/gtdprbihly.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtzojrjomh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gotoacloud.top/gtrevaimty.html

PHP:  array_merge(...$nested);
来源：http://hz.gzhubu.top/gtfiyhxmic.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gttkslmtqk.html

TS:   nested.flat();
来源：http://hz.guowangkeji.top/gtvyevdcys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dianchejie.cn/gtsgcyzxod.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtcnazwdpm.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtkynsorlj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cucudq.cn/gtdatkajtb.html

[D19] 按字段分组
来源：http://hz.meibo888.top/gtbglnbtke.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinyuanbaomall.cn/gtwihmofgm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.0kj1m.cn/gtngkmkbgj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sxryk.cn/gtltwdlvit.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtrahyoyqn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.mhx1999.top/gtoyzjunkt.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigfzy.top/gtmqwnmpyr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shanyushiyangtech.top/gthnqlkljv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gtmwedpptb.html

[D20] 统计每个元素出现次数
来源：http://hz.aibaodan.cn/gtuwenesvc.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtzlfkgkhl.html

PHP:  array_count_values($arr);
来源：http://hz.andypj.xyz/gtddazekms.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigufen.top/gtnxynovrh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtspyjupng.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cashguo.top/gttmkhfect.html

Go:   // 手写 map[T]int
来源：http://hz.yj202588.top/gtttcfcuzd.html

Ruby: arr.tally
来源：http://hz.xziqi.cn/gtgyiokjxd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jianghu66.top/gtjicuvayb.html

[D21] 判断是否包含某元素
来源：http://hz.hnxiangtu.top/gtwyuezcur.html

Py:   x in arr
来源：http://hz.shangyingyoupin.top/gtiothsaym.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ywan-chungtsiang.top/gtkipsylqe.html

JS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtcgxqmvso.html

TS:   arr.includes(x)
来源：http://hz.cheryme.top/gtghufmexr.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gtsdfucraq.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigufen.top/gtqctxzfim.html

Ruby: arr.include?(x)
来源：http://hz.yj20258888.top/gtrhmkhqfq.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtkceekwep.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fzhhl.top/gthvzzyzms.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jiagoushi.top/gtrdyfnktj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xziqi.cn/gtohdouncn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sxryk.cn/gtsscwxdfe.html

TS:   [...arr];
来源：http://hz.shangyingyoupin.top/gtxddodzvc.html

Java: new ArrayList<>(list);
来源：http://hz.snrcjt.cn/gtoonldjlv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.52xcode.cn/gtdbfdusmv.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gterzawgeh.html

C#:   new List<int>(list);
来源：http://hz.iojbl.cn/gtzvqosrya.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gthvncllqg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtcxptzzdu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nwbrower.top/gtrlslmiwz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtmibjzare.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgufenzy.top/gtvldbghun.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gthrhmbzki.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gthbogewqh.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtaxsanzfy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.pengpengdd.cyou/gteknwnjaw.html

[D24] 字典 / Map 基本操作
来源：http://hz.andypj.xyz/gtjbibvikq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.316326.xyz/gtegrfgroe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinyuanbaomall.cn/gtlucsyxhp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.haohaochexian.top/gtupseoucb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.mhx1999.top/gtrewyvfbq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtfwcakuub.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtgviblxsk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtrlwuhvgx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gtxheqgjvu.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtknvjlqbm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtttfpfmun.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtixncsozl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.nwbrower.top/gtarpvsiwd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtauylzaid.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hysaishi.cn/gtnmhlxrjx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gotoacloud.top/gtbjtrfkit.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhijiandao.cn/gtlbqihzwe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.svipenyu.cn/gtothluikk.html

[D26] 数组转字符串
来源：http://hz.xuetiantiany.cn/gtkcsosmez.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guannengcc.top/gtatzxjvox.html

PHP:  implode(", ", $arr);
来源：http://hz.jlsjyb.cn/gtbrqlpssl.html

JS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtsuvbtyvl.html

TS:   arr.join(", ")
来源：http://hz.bjfxy.top/gtbpyhplqb.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gtpmlisbqd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigufen.top/gtnuvukrhg.html

Ruby: arr.join(", ")
来源：http://hz.sxryk.cn/gtvmnaqqzq.html

C#:   string.Join(", ", list)
来源：http://hz.cqqwz.cn/gtgnhhislt.html

================================================================================
来源：http://hz.jyoumei.cn/gtmfsqctun.html

E. 字符串处理
来源：http://hz.pycfn.com/gtqthyhrow.html

================================================================================
来源：http://hz.hfpthk.cn/gttsyosioi.html

[E01] 拼接字符串
来源：http://hz.sysykeji.top/gtbqzoqwqf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.snrcjt.cn/gtstwogahp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.haohaochexian.top/gtsxmgyjuh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtguibcqss.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtqgnyrpaq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yangfankeji.com/gtolqymbfg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cqqwz.cn/gtqssjvyfl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangdashe.top/gtltcbjdir.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtktipdmvb.html

[E02] 重复字符串
来源：http://hz.yonumen.top/gtuziuxble.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtrzmjdldx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gtkmhepalq.html

JS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtdwmutmuw.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtcsxkvyjf.html

Java: "ab".repeat(3)
来源：http://hz.aizwys.cn/gtujxsrsyb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuanzx.com/gttmxljetp.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtkgqylsxt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtjuchicxe.html

[E03] 截取子串
来源：http://hz.yj202588.top/gtckdfwtek.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.52xcode.cn/gtsyzjhbpb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.feifeiyinyue.top/gttxaxyfgw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.birdmap.top/gttcymiccv.html

TS:   s.slice(1, 4)
来源：http://hz.sufxvd.cn/gtdbvuyvqq.html

Java: s.substring(1, 4)
来源：http://hz.yanxiufei.cn/gtiqemeyvi.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.birdmap.top/gtljshlppc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.wangdashe.top/gtnkxhzezu.html

C#:   s.Substring(1, 3)
来源：http://hz.hysaishi.cn/gtcqwszdyo.html

[E04] 查找子串位置
来源：http://hz.hywenlv.cn/gtwhjoggqk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhengqikj.top/gtmfwyqwfc.html

PHP:  strpos($s, "x");
来源：http://hz.shzxlz.cn/gtwujbjkxv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ppjwa.cn/gtbolusqwy.html

TS:   s.indexOf("x")
来源：http://hz.cdnleiting.top/gtxmxouuvb.html

Java: s.indexOf("x")
来源：http://hz.hysaishi.cn/gtdkkjnxto.html

Go:   strings.Index(s, "x")
来源：http://hz.xingfuxueyuan.xyz/gtidkfeizt.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtjnxlyhbg.html

C#:   s.IndexOf("x")
来源：http://hz.daxiang520.top/gtxibgunml.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.daxiang520.top/gtaidnybau.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtzxxuiozj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigufen.top/gtngvkvoup.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtzoupdvmk.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cashguo.top/gtjlbobfih.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuxming.cn/gteyrcdxxt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtwlgdiypq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.tian-w.cn/gtbbhhfgpk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.meibo888.top/gtzfqolivi.html

[E06] 替换子串
来源：http://hz.chenlongwang.top/gtlbhyqzna.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gtgqmmkbhe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pengpengdd.cyou/gtkqopzthy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinyuanbaomall.cn/gtzkcwkhzp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtsnawtpaa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtbfakeguo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtwxkzpjdc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zycfv.cn/gtvfzthhcd.html

C#:   s.Replace("a", "b")
来源：http://hz.sweek.top/gttasksksb.html

[E07] 按分隔符拆分
来源：http://hz.nwbrower.top/gtaaiimgva.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtarzpgykz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.feifeiyinyue.top/gtxfetzjkm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtaefgaaqf.html

TS:   s.split(",")
来源：http://hz.ivvv.top/gtfknvnfsv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.bjfxy.top/gtwrorbpta.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.andypj.xyz/gtctjwwyyo.html

Ruby: s.split(",");  s.split
来源：http://hz.gzhubu.top/gtefdipffk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtopyegeee.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtgnbeduzh.html

Py:   ",".join(items)
来源：http://hz.shzxlz.cn/gtogdpzraw.html

PHP:  implode(",", $items);
来源：http://hz.gogol.net.cn/gtyhxutyca.html

JS:   items.join(",")
来源：http://hz.316326.xyz/gteayhhquk.html

TS:   items.join(",")
来源：http://hz.jqgufenzy.top/gticixhrib.html

Java: String.join(",", items)
来源：http://hz.xziqi.cn/gtxyllwspk.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtddypvddj.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gthogxvrri.html

C#:   string.Join(",", items)
来源：http://hz.zhoulong.xyz/gtsykvwoyl.html

[E09] 去除所有空白字符
来源：http://hz.yj202588.top/gtzuruiqge.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtppzeiagn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtqikqvqri.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtsntxmqsj.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtkwgybksu.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jyoumei.cn/gtasokannw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yueranfly.top/gtcfxsubmh.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.tianlin.xyz/gtjaowelme.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gtiiruetmh.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sufxvd.cn/gtwfrckuin.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtbvimqmax.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.iojbl.cn/gtetpjexnn.html

JS:   "7".padStart(3, "0")
来源：http://hz.shuidangran.top/gtuqgdvdfm.html

TS:   "7".padStart(3, "0")
来源：http://hz.cqqwz.cn/gtomzbbfhr.html

Java: String.format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtccdawqdu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.guowangkeji.top/gtzzvhrwol.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tianlin.xyz/gtjtpzinlk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtbnzgzrvf.html

[E11] 反转字符串
来源：http://hz.zhiwuduotai.top/gtbtetugfu.html

Py:   s[::-1]
来源：http://hz.andypj.xyz/gtpunbwotp.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gtkezeuinc.html

JS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gtctoypomr.html

TS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gthlnupxre.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.feifeiyinyue.top/gtwscpjpnb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zycfv.cn/gtbnfzgtzu.html

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtoccvzvaq.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhongyouzk.top/gtlsvysonc.html

[E12] 统计某字符出现次数
来源：http://hz.sufxvd.cn/gtceanctsx.html

Py:   s.count("a")
来源：http://hz.zhongyouzk.top/gtgnvhudhz.html

PHP:  substr_count($s, "a");
来源：http://hz.yonumen.top/gtcdpaigod.html

JS:   s.split("a").length - 1
来源：http://hz.hammf.cn/gtpqxpsunq.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtzfcunmkj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ybcxt.top/gtspkzxoym.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtmoxezztj.html

Ruby: s.count("a")
来源：http://hz.jqgfzy.top/gthsdtxbvq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtcofpbpyj.html

[E13] 逐字符遍历
来源：http://hz.gotoacloud.top/gtdxlfrkji.html

Py:   for ch in s: print(ch)
来源：http://hz.0kj1m.cn/gtohpyqfnv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.dashuyun.cn/gtctffarlw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.tianlin.xyz/gtsoehhyqu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtufibromr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hammf.cn/gtbbbfrfxd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yanxiufei.cn/gtmsjxozgj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zycfv.cn/gtzajsmgor.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.mhx1999.top/gtseekohpc.html

[E14] URL 编码与 Base64
来源：http://hz.guowangkeji.top/gtowmiovbc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jinqigfzy.top/gteocdvzcf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.ywan-chungtsiang.top/gtquzbeayy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.jinyuanbaomall.cn/gtgtpysqua.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigfzy.top/gtsqcxcaum.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtypxbmxpv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.nwbrower.top/gtwircjozs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ppjwa.cn/gtueahxqwp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.shzxlz.cn/gtbxcmqgsz.html

[E15] HTML 转义 / 反转义
来源：http://hz.aizwys.cn/gtfterkwbq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.yuanzhike.top/gthdgqrwbv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hnqzz.top/gtwuuygmax.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gaohongyu789.top/gtcpqohbwg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xuanzx.com/gtjacpnvbb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shanyushiyangtech.top/gtgkwxqblp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jqgfzy.top/gtrzmkzqbq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xinyue.icu/gtwkphqlja.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yonumen.top/gtkvmqcemq.html

[E16] 数字千分位
来源：http://hz.jlsjyb.cn/gtyhlpcajp.html

Py:   f"{1234567:,}"
来源：http://hz.yangfankeji.com/gtdielxmdk.html

PHP:  number_format(1234567);
来源：http://hz.shzxlz.cn/gtttgqkine.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ppjwa.cn/gtcychirxc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtlggjcncd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daria6918.cn/gtluukvzso.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gtfyydriym.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.ybcxt.top/gtfnrynuos.html

C#:   1234567.ToString("N0")
来源：http://hz.yuanzhike.top/gtpazhpilm.html

[E17] 首字母大写
来源：http://hz.ydzc1.top/gtqrywoqwk.html


<!-- 参考信息 -->