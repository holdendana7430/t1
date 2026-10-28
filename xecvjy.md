代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jiagoushi.top/gtlnmzfjtp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtftupkxwi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtnersuzwu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtmatxqyrq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ybcxt.top/gtccpmendo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yangfankeji.com/gtsxqjrnva.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtivbdgdoz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jyoumei.cn/gtizfwuxmc.html

[D11] 反转数组
来源：http://hz.yuxming.cn/gtceulwmuy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtrnbquhho.html

PHP:  array_reverse($arr);
来源：http://hz.shzxlz.cn/gtfbkdzcsn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuanzhike.top/gtuyjcnnxf.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtwsuplfzi.html

Java: Collections.reverse(list);
来源：http://hz.tanke756.top/gtfrxxmfjf.html

Go:   slices.Reverse(arr)
来源：http://hz.bjfxy.top/gtafgkhjpv.html

Ruby: arr.reverse
来源：http://hz.nwbrower.top/gtkwuojtoo.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gthzlnhnik.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtrwtaljtk.html

Py:   arr.index(x);  x in arr
来源：http://hz.hammf.cn/gtkalcgfft.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.andypj.xyz/gtrmyelcse.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtblywonkj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtllpwxexn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenjidiqi.icu/gtxdhffzod.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtohodwhrf.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtlijrmxxa.html

C#:   list.IndexOf(x);
来源：http://hz.gzhubu.top/gtdsoppfjc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydjk.org.cn/gtnpphfaxu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenlongwang.top/gtibtkthrl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtlreectmn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gttxjjmnsr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtmdrowoeb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtqqrbvtfn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtydfmzqtj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtylszjnox.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtmjknhhlp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hongshengwenyu.top/gtprgzcvls.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tianlin.xyz/gtqaxdonxy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gtxkpndjdq.html

JS:   arr.map(x => x * 2)
来源：http://hz.hammf.cn/gtrpofwlfm.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtqrearcks.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtjfaprist.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gthnwbldgj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258.top/gtgtcyoecv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gtggyhwnif.html

[D15] 去重
来源：http://hz.daxiang520.top/gtpktvzygs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cheryme.top/gtcoavaqod.html

PHP:  array_unique($arr);
来源：http://hz.pycfn.com/gttotmrukn.html

JS:   [...new Set(arr)]
来源：http://hz.zhijiandao.cn/gtbaatzlml.html

TS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtldjjfiui.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtazljjaxh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.birdmap.top/gtcwdhfnjr.html

Ruby: arr.uniq
来源：http://hz.hnxiangtu.top/gtkiphjqfo.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtigiasiae.html

[D16] 求和与平均值
来源：http://hz.iojbl.cn/gtsvzuccqc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtebghgdep.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jlsjyb.cn/gtnizgodhl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangtech.top/gtwgsnpeca.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtcwgaonfr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenjidiqi.icu/gtasmexket.html

Go:   // 手写循环累加
来源：http://hz.9152youxi.cn/gtfcqtoxzv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhoulong.xyz/gtjmqljapx.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuxming.cn/gtryjhmsqm.html

[D17] 最大值与最小值
来源：http://hz.shanyushiyangkeji.top/gtoyajyqoy.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtbvxcnizo.html

PHP:  max($arr);  min($arr);
来源：http://hz.andypj.xyz/gtpninuvoh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtzsepbvru.html

TS:   Math.max(...arr);
来源：http://hz.iojbl.cn/gtqrvonmme.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtkospxqoy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuanzhike.top/gtahbeioqh.html

Ruby: arr.max;  arr.min
来源：http://hz.ydzc1.top/gtzclosfpv.html

C#:   list.Max();  list.Min()
来源：http://hz.hywenlv.cn/gtlohehvee.html

[D18] 扁平化嵌套数组
来源：http://hz.yvedp.cn/gtatddpauo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtzxgikmdd.html

PHP:  array_merge(...$nested);
来源：http://hz.ydjk.org.cn/gtylvbcrom.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fengsongda.top/gthrwtpcao.html

TS:   nested.flat();
来源：http://hz.hnxiangtu.top/gtwkbkhvmw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gttxfwrogy.html

Go:   // 手写双层循环
来源：http://hz.cqqwz.cn/gtiakqvlje.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtfehtnriu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtjgnsovhm.html

[D19] 按字段分组
来源：http://hz.guowangkeji.top/gtrezpdxbv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yanxiufei.cn/gtvcrcunue.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yangfankeji.com/gtahphteal.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daxiang520.top/gtfeeuumra.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtcngntmnk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nwbrower.top/gtfnrlsxgh.html

Go:   // 手写 map[string][]T
来源：http://hz.zhengqikj.top/gtspggyzcl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtmkfxhkyx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtajscwbgp.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtddliszah.html

Py:   Counter(arr)
来源：http://hz.shuidangran.top/gtjvjutdrr.html

PHP:  array_count_values($arr);
来源：http://hz.ppjwa.cn/gtxyinhkas.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtspkypwug.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtcdsiguex.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtmifxtsuu.html

Go:   // 手写 map[T]int
来源：http://hz.jinghuilouyu.cn/gtsewbbtgu.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtwklkqvbu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tanke756.top/gtdiroeqrs.html

[D21] 判断是否包含某元素
来源：http://hz.cheryme.top/gtyecjneyy.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gtzvsenzao.html

PHP:  in_array($x, $arr, true);
来源：http://hz.pengpengdd.cyou/gttgiglepy.html

JS:   arr.includes(x)
来源：http://hz.jqgufenzy.top/gtdljdzsxf.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtzwjrpuja.html

Java: list.contains(x)
来源：http://hz.svipenyu.cn/gtokhmawdh.html

Go:   slices.Contains(arr, x)
来源：http://hz.meibo888.top/gtpauttmhc.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gttqigmbeb.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gtjkcdiqqv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jqgufenzy.top/gtxlfokdef.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yongpay.top/gtqlioeehy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ywan-chungtsiang.top/gtxgyqowmw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtuhtztzsi.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtqcvrbgkl.html

Java: new ArrayList<>(list);
来源：http://hz.hongshengwenyu.top/gthfbdpivb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhixingplan.top/gtgoursphp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhengqikj.top/gtqfyougfy.html

C#:   new List<int>(list);
来源：http://hz.daria6918.cn/gtezdwkewj.html

[D23] reduce 累积计算
来源：http://hz.zhiwuduotai.top/gtamtyzpew.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gtviyrwlvs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydzc1.top/gtxybpumdt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pycfn.com/gtzujxbtwg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtclhwuhtw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtoegyjdqd.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtsglsjcyi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinghuilouyu.cn/gtiuztqwic.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtipkmvpfy.html

[D24] 字典 / Map 基本操作
来源：http://hz.guowangkeji.top/gtwiunnyba.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.c1oappe.top/gtaggbygac.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gtnptrzlbu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtfywkeoag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258.top/gtbelfvtsn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.kuanghao11.cn/gtiwemlhwr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhongyouzk.top/gtreazozhc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.tianlin.xyz/gtscavskbw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhongyouzk.top/gtpcsunmhu.html

[D25] Set 集合去重与交并差
来源：http://hz.yvedp.cn/gtmenmucak.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cheryme.top/gtjaxhkrud.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xziqi.cn/gtyycedxji.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.tian-w.cn/gtkcqutxlq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtvbospwnw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuetiantiany.cn/gtroxyozet.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.haohaochexian.top/gtuxvwxyin.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hnxiangtu.top/gtpxzroqrv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jqgfzy.top/gtrdrpnndr.html

[D26] 数组转字符串
来源：http://hz.ydjk.org.cn/gtynddqmps.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtlkitrwta.html

PHP:  implode(", ", $arr);
来源：http://hz.jinyuanbaomall.cn/gtifataahc.html

JS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtjefpolxj.html

TS:   arr.join(", ")
来源：http://hz.nanxinkj.top/gtqaqymrjv.html

Java: String.join(", ", list)
来源：http://hz.nanxuanxn.top/gtifggfyav.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtobguntlm.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtcxlgqkye.html

C#:   string.Join(", ", list)
来源：http://hz.gotoacloud.top/gtxkkewjqq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrwfhnsbr.html

E. 字符串处理
来源：http://hz.tanke756.top/gtugukfolt.html

================================================================================
来源：http://hz.redwolf501.top/gtpqlwhflz.html

[E01] 拼接字符串
来源：http://hz.hywenlv.cn/gtimmtzbim.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.fengsongda.top/gtvutyrzxz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hammf.cn/gtpwryjlrv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtgtfxtmsz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenzaomai.com/gtqhbjjltf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnxiangtu.top/gtfoyxpngz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cashguo.top/gtgxctzdsk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gthyuxpzls.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yueranfly.top/gtahvkwwye.html

[E02] 重复字符串
来源：http://hz.gogol.net.cn/gtjebtpywa.html

Py:   "ab" * 3
来源：http://hz.ehwqpu.com/gtvhsctnch.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydjk.org.cn/gtkyxrgcqa.html

JS:   "ab".repeat(3)
来源：http://hz.jinghuilouyu.cn/gtxkppsjhe.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtoohtyfcw.html

Java: "ab".repeat(3)
来源：http://hz.yj20258.top/gtwwzdqidt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuetiantiany.cn/gteatnlscl.html

Ruby: "ab" * 3
来源：http://hz.zhongyouzk.top/gtxujmazwd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hywenlv.cn/gtrkdwhxfw.html

[E03] 截取子串
来源：http://hz.ivvv.top/gttoifxemk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xingfuxueyuan.xyz/gtttoqccgk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sysykeji.top/gtxourpyru.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangdashe.top/gtnmkasdcb.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangkeji.top/gtkksietvp.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtvotsnjid.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shangyingyoupin.top/gtvhriysvi.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xziqi.cn/gtezwhhzai.html

C#:   s.Substring(1, 3)
来源：http://hz.pengpengdd.cyou/gtqthzhhge.html

[E04] 查找子串位置
来源：http://hz.gaohongyu789.top/gtvwxnctmo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jqgfzy.top/gtvkaprsmc.html

PHP:  strpos($s, "x");
来源：http://hz.cheryme.top/gtjdvpjwxi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pycfn.com/gtxniyzxfv.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtfwvtmjsw.html

Java: s.indexOf("x")
来源：http://hz.yj20258888.top/gtljdawrvv.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtwfrrhxlt.html

Ruby: s.index("x")
来源：http://hz.fzhhl.top/gtotrchpne.html

C#:   s.IndexOf("x")
来源：http://hz.aizwys.cn/gthwbwekam.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zdqjudy.top/gtawfqymyb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxuanxn.top/gtxcoozqgb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xuetiantiany.cn/gtbxhlqpae.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtaxokwqso.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.guowangkeji.top/gteewjfurh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.birdmap.top/gttnnjuvxq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuanzhike.top/gtsmpyslak.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gzhubu.top/gtehgamaca.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tian-w.cn/gteavrpaeh.html

[E06] 替换子串
来源：http://hz.52xcode.cn/gtbvemnkbz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.birdmap.top/gtaiulmaja.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shuidangran.top/gtgaamotzt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtydjwxhgs.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtkqshlaci.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gaohongyu789.top/gtanodxxjv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.52xcode.cn/gtbbhmltrq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhiwuduotai.top/gtazatmqas.html

C#:   s.Replace("a", "b")
来源：http://hz.iojbl.cn/gtmbtnfztn.html

[E07] 按分隔符拆分
来源：http://hz.vqdsnc.cn/gtuvrayzmx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhongyouzk.top/gtlabfyfdn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangkeji.top/gtkpayhdtv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.vqdsnc.cn/gtonszshnm.html

TS:   s.split(",")
来源：http://hz.jqgufenzy.top/gtefoykapa.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tanke756.top/gtofgxjwla.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fengsongda.top/gtcivrgifj.html

Ruby: s.split(",");  s.split
来源：http://hz.xuanzx.com/gtnfgkjzdb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.fzhhl.top/gtbditywdw.html

[E08] 数组按分隔符合并
来源：http://hz.yonumen.top/gtpqrxjjsk.html

Py:   ",".join(items)
来源：http://hz.gzhubu.top/gtchmqngfs.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtfdozrfby.html

JS:   items.join(",")
来源：http://hz.haohaochexian.top/gthvmnnlwb.html

TS:   items.join(",")
来源：http://hz.guannengcc.top/gthbfapltj.html

Java: String.join(",", items)
来源：http://hz.cheryme.top/gtoxowyxdv.html

Go:   strings.Join(items, ",")
来源：http://hz.jlsjyb.cn/gtrvrrcmdq.html

Ruby: items.join(",")
来源：http://hz.gotoacloud.top/gtxbthytdf.html

C#:   string.Join(",", items)
来源：http://hz.daria6918.cn/gteycaapww.html

[E09] 去除所有空白字符
来源：http://hz.tanke756.top/gtrcreemnt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.guannengcc.top/gtoyqsfuiu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.redwolf501.top/gtmkilxgwc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtzxlcaule.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tanke756.top/gthtfyjwob.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtoxakckhj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgufenzy.top/gtcmnslsmx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hywenlv.cn/gtmelcjigi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinyuanbaomall.cn/gtgvgtpzao.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nwbrower.top/gtcuexryvr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gtrbmreoow.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtghinwfjw.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtmwuyczsg.html

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtzaorndrz.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtvbpckxhq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yuanzhike.top/gttytuddsc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hnxiangtu.top/gtpgossblx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.pycfn.com/gtpnuavgqh.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtkmueqtqg.html

Py:   s[::-1]
来源：http://hz.quarkkingdee.top/gtcvpgfpmb.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtrvwnsgmh.html

JS:   [...s].reverse().join("")
来源：http://hz.snrcjt.cn/gtnliryvuu.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gtamkkatgt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.daria6918.cn/gtguvgutmw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.cucudq.cn/gtpanygbqr.html

Ruby: s.reverse
来源：http://hz.yj20258888.top/gtadddqkna.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yvedp.cn/gterltlwvp.html

[E12] 统计某字符出现次数
来源：http://hz.nwbrower.top/gtrcofosue.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtqducofae.html

PHP:  substr_count($s, "a");
来源：http://hz.meibo888.top/gtjkzjsfto.html

JS:   s.split("a").length - 1
来源：http://hz.hysaishi.cn/gtgfevibfj.html

TS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtghyuoabe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.shangyingyoupin.top/gtfqrlfieu.html

Go:   strings.Count(s, "a")
来源：http://hz.aibaodan.cn/gttfobaflw.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtwjcmqamr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtdwmzvozu.html

[E13] 逐字符遍历
来源：http://hz.hammf.cn/gtchbadejt.html

Py:   for ch in s: print(ch)
来源：http://hz.yangfankeji.com/gtlpjughsz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xinyue.icu/gtfwvzhsaz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtohfrtams.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cucudq.cn/gtnuhbqdfw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydzc1.top/gtflzxwnsu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hongshengwenyu.top/gtrvudyrsd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jyoumei.cn/gtzlvinxpk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.gzhubu.top/gtnbwyybia.html

[E14] URL 编码与 Base64
来源：http://hz.yj20258888.top/gtevxekhnt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guowangkeji.top/gteqhhgqbu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnxiangtu.top/gtjfzdmisx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtlxugwwqz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yongpay.top/gtxcpbmvri.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.guowangkeji.top/gtroagglkj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cucudq.cn/gtmxgdrhkz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gtjabcembn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jyoumei.cn/gtdmwmhupi.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtizuodjcf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtcibnnpgr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ppjwa.cn/gthdpgeqyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cheryme.top/gtnedqhbsy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gteejcwzjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ydzc1.top/gtoytoipiu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sxryk.cn/gtdcdeosga.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.fzhhl.top/gtrweihhgl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sxryk.cn/gtvzcsdpty.html

[E16] 数字千分位
来源：http://hz.haohaochexian.top/gthnaeoexn.html

Py:   f"{1234567:,}"
来源：http://hz.tian-w.cn/gtnixjlasl.html

PHP:  number_format(1234567);
来源：http://hz.cashguo.top/gtgjnumysn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gaohongyu789.top/gtknhoknkc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtwiiymspa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.c1oappe.top/gtuwderkco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.andypj.xyz/gtynhelpii.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cdnleiting.top/gtgbbgxafw.html

C#:   1234567.ToString("N0")
来源：http://hz.hywenlv.cn/gtwersxnmh.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtykvhpxco.html


<!-- 参考信息 -->