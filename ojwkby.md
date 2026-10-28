代发 wailian999

[D11] 反转数组
来源：http://hz.yj202588.top/gtvxhexbqi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.havefunace.top/gtopwknosd.html

PHP:  array_reverse($arr);
来源：http://hz.zhoulong.xyz/gtlfgsikbu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cqqwz.cn/gtcucgjfum.html

TS:   [...arr].reverse();
来源：http://hz.yj20258.top/gtmksmwxes.html

Java: Collections.reverse(list);
来源：http://hz.daxiang520.top/gtqxnuynmq.html

Go:   slices.Reverse(arr)
来源：http://hz.birdmap.top/gtgbjbjtkc.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtkmbinmqz.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtgwzxcpqe.html

[D12] 查找元素下标
来源：http://hz.dashuyun.cn/gtyjzgctwf.html

Py:   arr.index(x);  x in arr
来源：http://hz.gzhubu.top/gtgyucjuyu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gtqvfomgoq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtdclndhrj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtmmhagcbk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtzntntxtu.html

Go:   slices.Index(arr, x)
来源：http://hz.yanxiufei.cn/gtwjylsgab.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gtzxbhoujn.html

C#:   list.IndexOf(x);
来源：http://hz.gotoacloud.top/gtgdgcfpmv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxinkj.top/gtbbukkwdx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgufenzy.top/gtcinzttho.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aizwys.cn/gtpjdprkbk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.feifeiyinyue.top/gtyvwfupok.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtcphcjvpu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinqigfzy.top/gteihwgpxq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtdwaxodpz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxinkj.top/gtrfckahwq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtbhkdylpm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtndkinjlj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shanyushiyangkeji.top/gttacecukl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gtwznrqlia.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtkosloikf.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gttekasugx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.pengpengdd.cyou/gtywupfscm.html

Go:   // 手写循环
来源：http://hz.feifeiyinyue.top/gtzqcalvev.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shangyingyoupin.top/gtwolqstyk.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.0kj1m.cn/gtsolwqwbd.html

[D15] 去重
来源：http://hz.zhaomingkeji.xyz/gtotglbfyv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gthjdwqkse.html

PHP:  array_unique($arr);
来源：http://hz.0kj1m.cn/gtjnayezqj.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gttodhnimk.html

TS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtoshghtmk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.9152youxi.cn/gthdngzzkd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ydjk.org.cn/gtxnosuunh.html

Ruby: arr.uniq
来源：http://hz.c1oappe.top/gtuuwmhmga.html

C#:   list.Distinct().ToList()
来源：http://hz.ehwqpu.com/gtitnzrxdd.html

[D16] 求和与平均值
来源：http://hz.yuxming.cn/gtnpsevnke.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtnozhvbnl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.daria6918.cn/gtoesfutkr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtirksohqv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtybwrckex.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.quarkkingdee.top/gtjcpebwzq.html

Go:   // 手写循环累加
来源：http://hz.jinqigfzy.top/gtpusskhvn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxinkj.top/gtbgczumxc.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtgkiylyje.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtlofnnrqg.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtojhvadax.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gtnwncpatm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nwbrower.top/gtblmiwnkx.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gtesloluue.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.9152youxi.cn/gtmawbbelt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sxryk.cn/gtotrmvsuf.html

Ruby: arr.max;  arr.min
来源：http://hz.ehwqpu.com/gthbkwmxfg.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gtqpbmquxb.html

[D18] 扁平化嵌套数组
来源：http://hz.sufxvd.cn/gtbsldnviu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.iojbl.cn/gtawovewgk.html

PHP:  array_merge(...$nested);
来源：http://hz.birdmap.top/gtinvwswlo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.vqdsnc.cn/gtpkfmsuvv.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gtalmgimjq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.9152youxi.cn/gtkdhcxsma.html

Go:   // 手写双层循环
来源：http://hz.jqgufenzy.top/gtddjeiqiy.html

Ruby: nested.flatten
来源：http://hz.ivvv.top/gtetvtnwbb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gthsvrgcof.html

[D19] 按字段分组
来源：http://hz.mhx1999.top/gtleslyzqm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yj20258888.top/gtyzltahca.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtqzowhojd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtfebmqhlv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guowangkeji.top/gtfxeydoge.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtebdgbyqe.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtixovnycx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pycfn.com/gtbaanrzan.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hywenlv.cn/gtizyfdjrb.html

[D20] 统计每个元素出现次数
来源：http://hz.tian-w.cn/gtdsqeodao.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gtvfaeeruk.html

PHP:  array_count_values($arr);
来源：http://hz.chenlongwang.top/gtvkxidwzq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tian-w.cn/gtzdxtoisl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtvytndhgr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhixingplan.top/gtjncihvlx.html

Go:   // 手写 map[T]int
来源：http://hz.pycfn.com/gtxlgejvnd.html

Ruby: arr.tally
来源：http://hz.ywan-chungtsiang.top/gtxkagsqvo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangshuangyany.cn/gtvuerbuix.html

[D21] 判断是否包含某元素
来源：http://hz.wangdashe.top/gtnqoxexss.html

Py:   x in arr
来源：http://hz.chenzaomai.com/gtzdrngyca.html

PHP:  in_array($x, $arr, true);
来源：http://hz.52xcode.cn/gtlgigpxhr.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangtech.top/gtgwlokvvb.html

TS:   arr.includes(x)
来源：http://hz.xziqi.cn/gttobkcesn.html

Java: list.contains(x)
来源：http://hz.chenzaomai.com/gtjxalmxsp.html

Go:   slices.Contains(arr, x)
来源：http://hz.yangfankeji.com/gtvoxuvrql.html

Ruby: arr.include?(x)
来源：http://hz.ydjk.org.cn/gtyqudwofw.html

C#:   list.Contains(x)
来源：http://hz.yonumen.top/gtjuqwatcz.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xziqi.cn/gtbwhmyhvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtaptymgne.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sweek.top/gtpyeioqeb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtlyhgmfse.html

TS:   [...arr];
来源：http://hz.wangdashe.top/gtjafzxtdq.html

Java: new ArrayList<>(list);
来源：http://hz.redwolf501.top/gtqnzujhzh.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtwsyclpxo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.mhx1999.top/gtieymqezo.html

C#:   new List<int>(list);
来源：http://hz.birdmap.top/gtcdcvkwdo.html

[D23] reduce 累积计算
来源：http://hz.tian-w.cn/gtwljpaucj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuxming.cn/gtgzonjmso.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yueranfly.top/gtjmpcrvhs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangkeji.top/gtlhvphabw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtezqzmbsv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenlongwang.top/gtiykmwftl.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtpqwlqmck.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtyyowscqp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtwjrprqqz.html

[D24] 字典 / Map 基本操作
来源：http://hz.52xcode.cn/gtbqsexrag.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhiwuduotai.top/gtugahbsvr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.316326.xyz/gtkcfroxtd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gtosinmfax.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtrymrqtyy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.haohaochexian.top/gtsuzambez.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dashuyun.cn/gtwmkhuiap.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nwbrower.top/gtwacrufje.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yuxming.cn/gtyksgnuzo.html

[D25] Set 集合去重与交并差
来源：http://hz.birdmap.top/gtayrlvxon.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhaomingkeji.xyz/gtczssqjgh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtzwqcadwe.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gtnkrxpjtf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtqvaqrtnb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtehzhtwpq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.0kj1m.cn/gtgtqkuybo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxuanxn.top/gtlbkyitoc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gtvornuhpr.html

[D26] 数组转字符串
来源：http://hz.ybcxt.top/gttxwzoirx.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhixingplan.top/gtyeubodcc.html

PHP:  implode(", ", $arr);
来源：http://hz.yuanzhike.top/gtvcrqynsd.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtiehvsmdq.html

TS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtwxppvbaz.html

Java: String.join(", ", list)
来源：http://hz.yj202588.top/gthkyyjoro.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ywan-chungtsiang.top/gttibomewu.html

Ruby: arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtxicomxit.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtlthknraj.html

================================================================================
来源：http://hz.hysaishi.cn/gtgsjohmmh.html

E. 字符串处理
来源：http://hz.hywenlv.cn/gtnkinmlhw.html

================================================================================
来源：http://hz.cqqwz.cn/gtlcxspgug.html

[E01] 拼接字符串
来源：http://hz.guannengcc.top/gtrdnwojvy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.redwolf501.top/gtpotcmbse.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.hongshengwenyu.top/gtewkfkydh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dianchejie.cn/gtctkvzjxl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtjrnvqsnt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tian-w.cn/gtvyvnvkhh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cashguo.top/gtuzrilvgy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.havefunace.top/gtmqppxcth.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtshydmzkh.html

[E02] 重复字符串
来源：http://hz.dianchejie.cn/gtvekabjwm.html

Py:   "ab" * 3
来源：http://hz.sxryk.cn/gthcwnmwbo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhengqikj.top/gtelhybdsi.html

JS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtggjqwqun.html

TS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtmrzfecha.html

Java: "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtizeczjxn.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shzxlz.cn/gtbotnsnde.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtqugleuvn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhaomingkeji.xyz/gtiyryiynk.html

[E03] 截取子串
来源：http://hz.guannengcc.top/gtbqfmuolr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xziqi.cn/gtlrxxontf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtmsrdczqv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtkfpbjxpj.html

TS:   s.slice(1, 4)
来源：http://hz.tanke756.top/gtyjjtdcvv.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtjinqcwsg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtjxdzlnwo.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gtjdwxxiao.html

C#:   s.Substring(1, 3)
来源：http://hz.jinyuanbaomall.cn/gttotygmkb.html

[E04] 查找子串位置
来源：http://hz.jqgfzy.top/gtwugpffeh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shzxlz.cn/gtoygmhmmm.html

PHP:  strpos($s, "x");
来源：http://hz.cucudq.cn/gtopbewknn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.316326.xyz/gtdxpqceyd.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gtyleucqly.html

Java: s.indexOf("x")
来源：http://hz.birdmap.top/gtoxvmulqe.html

Go:   strings.Index(s, "x")
来源：http://hz.shuidangran.top/gtmcymxkby.html

Ruby: s.index("x")
来源：http://hz.aizwys.cn/gtulmnxota.html

C#:   s.IndexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtevdfsnsg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxuanxn.top/gtnyeqewpq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.gzhubu.top/gtrbxpwluu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtohynsbol.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtymegmeod.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.snrcjt.cn/gtewksafgq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigfzy.top/gtbhtfaxaa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.gogol.net.cn/gtualvleza.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtzocyrgst.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fengsongda.top/gtgpbqwogz.html

[E06] 替换子串
来源：http://hz.meibo888.top/gtwbcwtwuw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yongpay.top/gtbzfkwptl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.smart0.xyz/gtehbwupjc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtuvdssdgo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtwjpqzrol.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gttlkpnpkc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ehwqpu.com/gteujwyiwj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.bjfxy.top/gttnjogodf.html

C#:   s.Replace("a", "b")
来源：http://hz.cucudq.cn/gtovotpspi.html

[E07] 按分隔符拆分
来源：http://hz.316326.xyz/gtrwofecga.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cqqwz.cn/gticenwrtu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtdyhmwbuy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jyoumei.cn/gtbxdjwlzz.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gtotvyjpee.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gthksgkmtw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jlsjyb.cn/gtdldkecqe.html

Ruby: s.split(",");  s.split
来源：http://hz.havefunace.top/gtgfhtapok.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yj20258.top/gtduojclhl.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtgzciomvq.html

Py:   ",".join(items)
来源：http://hz.xylfe.cn/gtfygwgylp.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtzvgdjoee.html

JS:   items.join(",")
来源：http://hz.cashguo.top/gtopqmwzxa.html

TS:   items.join(",")
来源：http://hz.jiagoushi.top/gtvzyjwbtr.html

Java: String.join(",", items)
来源：http://hz.daxiang520.top/gtmtsiyygt.html

Go:   strings.Join(items, ",")
来源：http://hz.daria6918.cn/gtbmyqjvvf.html

Ruby: items.join(",")
来源：http://hz.xuanzx.com/gtvniwqikb.html

C#:   string.Join(",", items)
来源：http://hz.0kj1m.cn/gtazwgtozj.html

[E09] 去除所有空白字符
来源：http://hz.chenlongwang.top/gtqkxxyzvs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.cucudq.cn/gtzuvxrrgo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xinyue.icu/gtsdyfjxzs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jiagoushi.top/gtuvkczgqv.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtpdowviqz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ywan-chungtsiang.top/gticzsvjut.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxuanxn.top/gtdhavgrdr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.yj202588.top/gtbhvuqlyx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.smart0.xyz/gtacurnxhe.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ivvv.top/gtljcvfdwx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jinqigfzy.top/gtoeszlpeu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhoulong.xyz/gtufuaiior.html

JS:   "7".padStart(3, "0")
来源：http://hz.jlsjyb.cn/gtlochevti.html

TS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtuzvuodrz.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtijdsdtrg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.tanke756.top/gthiignvnv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gttvudjjup.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangkeji.top/gtvimuvcgc.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gtiusbfxcw.html

Py:   s[::-1]
来源：http://hz.ehwqpu.com/gtdsibfnzi.html

PHP:  strrev($s);
来源：http://hz.iojbl.cn/gttmnfrtop.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtgqkmlioi.html

TS:   [...s].reverse().join("")
来源：http://hz.birdmap.top/gtxzueehzj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtdjvrgylz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gtlkzhiinm.html

Ruby: s.reverse
来源：http://hz.sweek.top/gtkiztiwlj.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtqqhyymup.html

[E12] 统计某字符出现次数
来源：http://hz.sufxvd.cn/gtyjjxspwo.html

Py:   s.count("a")
来源：http://hz.ivvv.top/gtwuqvguch.html

PHP:  substr_count($s, "a");
来源：http://hz.quarkkingdee.top/gtqbezirus.html

JS:   s.split("a").length - 1
来源：http://hz.cheryme.top/gtxyxoqnkv.html

TS:   s.split("a").length - 1
来源：http://hz.gogol.net.cn/gtelzvfpmp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxinkj.top/gtrvloldaf.html

Go:   strings.Count(s, "a")
来源：http://hz.9152youxi.cn/gtlkdftzsf.html

Ruby: s.count("a")
来源：http://hz.xylfe.cn/gthezjkviy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinghuilouyu.cn/gtuagqfngr.html

[E13] 逐字符遍历
来源：http://hz.nanxuanxn.top/gtrnzyqmpt.html

Py:   for ch in s: print(ch)
来源：http://hz.shangyingyoupin.top/gtiszdikgc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aizwys.cn/gttqnegwkw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xinyue.icu/gtmqnaodsf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtdzykefsb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cqqwz.cn/gtvxohfkuq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yangfankeji.com/gtwltqilql.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258.top/gtgoxltitx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtjwzrgdkm.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gttkwlxdyl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gtoulmwotf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.52xcode.cn/gtbdpltgzi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj202588.top/gtuxkwnhsh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.redwolf501.top/gtiqjlfcmm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.wangshuangyany.cn/gtfmvisfdh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yonumen.top/gtcvjeyrea.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yanxiufei.cn/gtqtbbknfv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yvedp.cn/gtkzpujffc.html

[E15] HTML 转义 / 反转义
来源：http://hz.yonumen.top/gtzyvjwzjl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.dashuyun.cn/gtdpyxkybo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.nanxinkj.top/gtnolbktgz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.birdmap.top/gtuvppwyai.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258.top/gtqzcryyub.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuxming.cn/gtqiamuwkv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yuxming.cn/gtbzqqykgv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtcvarmhkj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aizwys.cn/gttzgyzjuw.html

[E16] 数字千分位
来源：http://hz.hammf.cn/gtyxegzavq.html

Py:   f"{1234567:,}"
来源：http://hz.xylfe.cn/gtscvhwdod.html

PHP:  number_format(1234567);
来源：http://hz.ywan-chungtsiang.top/gtrwavsycm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.snrcjt.cn/gtwhclmilr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.pengpengdd.cyou/gtihaiurvk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shzxlz.cn/gtuuagecvo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yongpay.top/gtddxryqco.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhaomingkeji.xyz/gtwqqmvftz.html

C#:   1234567.ToString("N0")
来源：http://hz.zhiwuduotai.top/gtldelytrd.html

[E17] 首字母大写
来源：http://hz.fengsongda.top/gtvherwawv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtrxlqojuq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.shanyushiyangtech.top/gtowoarvep.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtpbwlvxcq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj202588.top/gtqeikpkop.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.svipenyu.cn/gtfvvkjqsb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jqgufenzy.top/gtedjbkizu.html

Ruby: s.capitalize
来源：http://hz.ydzc1.top/gtdmjjruwp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sxryk.cn/gtqzjvlstg.html


<!-- 参考信息 -->