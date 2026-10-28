代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtpasybsuk.html

TS:   [...a, ...b];
来源：http://hz.ybcxt.top/gtuowqkmod.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sxryk.cn/gtjatlparo.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtywatskgq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.smart0.xyz/gtbmdlsien.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtokigpcut.html

[D09] 排序（升序）
来源：http://hz.fzhhl.top/gtuftfpycy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtficpcyib.html

PHP:  sort($arr);
来源：http://hz.jqgufenzy.top/gtgqiabnsf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ivvv.top/gtdnokodhk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gthpsqkaba.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tanke756.top/gttskgwrgh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtedcokxxc.html

Ruby: arr.sort
来源：http://hz.quarkkingdee.top/gtkgmraftv.html

C#:   list.Sort();
来源：http://hz.dianchejie.cn/gtblcckcaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gtupofrjzn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtnyrtsltw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.redwolf501.top/gtudizyrru.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtbnegkikw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtzoyeudpq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tian-w.cn/gtibqqouhq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtgpmlqacn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gtwzjsznlu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.0kj1m.cn/gtrkvemhqw.html

[D11] 反转数组
来源：http://hz.tanke756.top/gtphdrcnvb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinqigfzy.top/gtzxuewney.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtzyzysjku.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhixingplan.top/gtovwdmnec.html

TS:   [...arr].reverse();
来源：http://hz.sweek.top/gtzjlmmedg.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtdxzatnvc.html

Go:   slices.Reverse(arr)
来源：http://hz.dianchejie.cn/gtelpbxzbs.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtevwqiyur.html

C#:   list.Reverse();
来源：http://hz.tian-w.cn/gtsjxeslxu.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtocvlkjbb.html

Py:   arr.index(x);  x in arr
来源：http://hz.shanyushiyangtech.top/gtviuspmyo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jyoumei.cn/gtzhnbcqxv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtqilfwhgq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtafqrhklv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhengqikj.top/gtixrluwiq.html

Go:   slices.Index(arr, x)
来源：http://hz.hfpthk.cn/gtrmpcobak.html

Ruby: arr.index(x)
来源：http://hz.yueranfly.top/gtudettczw.html

C#:   list.IndexOf(x);
来源：http://hz.zhongyouzk.top/gtrcjzlsyg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.pengpengdd.cyou/gtlqqaqaxy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.kuanghao11.cn/gtmgjyhyts.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aizwys.cn/gtijssgnuo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtnbexhasl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtyovaqtpz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gthjevwxnk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hammf.cn/gtaofpiqxh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnqzz.top/gtxqbijniv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pycfn.com/gtyqbvueyp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuanzhike.top/gtcmydlrsp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuanzx.com/gtmxvuhpma.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtpxyyjoae.html

JS:   arr.map(x => x * 2)
来源：http://hz.svipenyu.cn/gtflwrwxna.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtpwfhewyy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtyelgicvb.html

Go:   // 手写循环
来源：http://hz.shanyushiyangkeji.top/gtrkrczfme.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhengqikj.top/gtqaymcqpm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtikexvvxb.html

[D15] 去重
来源：http://hz.mhx1999.top/gtalsldhad.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtsfdqgtvy.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtnkzintvw.html

JS:   [...new Set(arr)]
来源：http://hz.52xcode.cn/gtzcotucqf.html

TS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtbiotwebk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenjidiqi.icu/gteooihuay.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtvrssrpek.html

Ruby: arr.uniq
来源：http://hz.gaohongyu789.top/gtydnhzlkp.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtsfgwqdox.html

[D16] 求和与平均值
来源：http://hz.jqgufenzy.top/gtsbovwcno.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cashguo.top/gtyydtzmbg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtcrmzmsam.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtzieouzhh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.smart0.xyz/gtltioozhu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhixingplan.top/gtfjpiueta.html

Go:   // 手写循环累加
来源：http://hz.xingfuxueyuan.xyz/gtadlyzgie.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cqqwz.cn/gteyjxlpwy.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtkbxfvthh.html

[D17] 最大值与最小值
来源：http://hz.yvedp.cn/gtbhgqhdnc.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gthbvohpkm.html

PHP:  max($arr);  min($arr);
来源：http://hz.9152youxi.cn/gtmfuonlhp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtgwelwufh.html

TS:   Math.max(...arr);
来源：http://hz.mhx1999.top/gthvrlyjex.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.snrcjt.cn/gtpfrmjfjy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtjgrmnnzv.html

Ruby: arr.max;  arr.min
来源：http://hz.tian-w.cn/gtvvyhgxtz.html

C#:   list.Max();  list.Min()
来源：http://hz.yonumen.top/gtsdvgtcfy.html

[D18] 扁平化嵌套数组
来源：http://hz.yj202588.top/gtgizumoaf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.pengpengdd.cyou/gtyukfawga.html

PHP:  array_merge(...$nested);
来源：http://hz.sxryk.cn/gtkbsvdkvm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtbeuhkspn.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtwykyyvcp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hysaishi.cn/gtddafpjfm.html

Go:   // 手写双层循环
来源：http://hz.hywenlv.cn/gtxzokdpvi.html

Ruby: nested.flatten
来源：http://hz.yueranfly.top/gtxlwmpngk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtvnxqpogs.html

[D19] 按字段分组
来源：http://hz.yj20258.top/gtduqbiaqq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cdnleiting.top/gttujvbnlg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuanzhike.top/gthemrdgoe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.kuanghao11.cn/gtkldsvytp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yangfankeji.com/gtpvplnckp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.iojbl.cn/gtckzjtyxn.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtgexgbmwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtajqppcmm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.andypj.xyz/gtlzovqvcy.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtnogzivex.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gtbcddgsva.html

PHP:  array_count_values($arr);
来源：http://hz.svipenyu.cn/gtfeqwwett.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shangyingyoupin.top/gtactxhrvl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nwbrower.top/gtbgqxflgq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtnmcztuaq.html

Go:   // 手写 map[T]int
来源：http://hz.smart0.xyz/gtonetbora.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtylawgqry.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258888.top/gtnpxwddge.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtxgvtifen.html

Py:   x in arr
来源：http://hz.zhengqikj.top/gtwrvtfaxu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtbctdbqgw.html

JS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtpzmowfls.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtnrdmuzap.html

Java: list.contains(x)
来源：http://hz.gotoacloud.top/gtxkplfeeq.html

Go:   slices.Contains(arr, x)
来源：http://hz.yanxiufei.cn/gtqzleuxrj.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gttooxymwc.html

C#:   list.Contains(x)
来源：http://hz.hnqzz.top/gtgbpzybon.html

[D22] 复制数组（避免共享引用）
来源：http://hz.andypj.xyz/gtxzkhvfab.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtcmhtsbfj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtpglelmyo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtgtrkzios.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtjyzcuqbr.html

Java: new ArrayList<>(list);
来源：http://hz.0kj1m.cn/gtcndjccje.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nanxuanxn.top/gtsjoyzhbg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cucudq.cn/gtaoteeipz.html

C#:   new List<int>(list);
来源：http://hz.c1oappe.top/gttotrtruo.html

[D23] reduce 累积计算
来源：http://hz.xingfuxueyuan.xyz/gtmkgddybh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.guowangkeji.top/gtfxwhkvvy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pengpengdd.cyou/gtrdzzthna.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.52xcode.cn/gttikmwojh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtpgyelkwa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dianchejie.cn/gtnyrtfhfp.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtfyahaous.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgfzy.top/gtfivcbyvq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtdspqymau.html

[D24] 字典 / Map 基本操作
来源：http://hz.iojbl.cn/gtpzfyofcs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtllsjiblt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.feifeiyinyue.top/gtrnlnxhqp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtplhvyuix.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.mhx1999.top/gtnpxawqwt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhijiandao.cn/gtdmldwsex.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jyoumei.cn/gtpctfvewc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.daria6918.cn/gtfaopqxsl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ydzc1.top/gtzbnuuwwg.html

[D25] Set 集合去重与交并差
来源：http://hz.jianghu66.top/gtzmgdoxph.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zycfv.cn/gtawxyfznh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.9152youxi.cn/gtpdmkswxs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtikuosdou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.aibaodan.cn/gtugwylpcu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtywqiohes.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.feifeiyinyue.top/gtecxrnsfv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.quarkkingdee.top/gtuirzxcay.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinyuanbaomall.cn/gtlacwrlqy.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtrixbchqm.html

Py:   ", ".join(map(str, arr))
来源：http://hz.redwolf501.top/gtyhwsyapn.html

PHP:  implode(", ", $arr);
来源：http://hz.shangyingyoupin.top/gtyhinfbqx.html

JS:   arr.join(", ")
来源：http://hz.vqdsnc.cn/gtjtkuyvxf.html

TS:   arr.join(", ")
来源：http://hz.c1oappe.top/gtkfbwxoya.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtpupqejxj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenjidiqi.icu/gtttqwvasc.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gtoqddczjo.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtxhharogr.html

================================================================================
来源：http://hz.bjfxy.top/gtnbjmsbzb.html

E. 字符串处理
来源：http://hz.daxiang520.top/gtmfurfgdy.html

================================================================================
来源：http://hz.yvedp.cn/gtuvghfrpf.html

[E01] 拼接字符串
来源：http://hz.yueranfly.top/gtgbzjtzbn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aizwys.cn/gtppddlqsc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhiwuduotai.top/gtqanpqrbj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xingfuxueyuan.xyz/gthxbbzzow.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtxjzfysvq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gtjfnpkhis.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtpmklgogz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cqqwz.cn/gtlsvegjek.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.guannengcc.top/gtzddmdvxk.html

[E02] 重复字符串
来源：http://hz.yanxiufei.cn/gtsntzuwww.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gtdeousbev.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yonumen.top/gtmoufslsh.html

JS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtkkesankk.html

TS:   "ab".repeat(3)
来源：http://hz.c1oappe.top/gtmyccgqve.html

Java: "ab".repeat(3)
来源：http://hz.xziqi.cn/gthaidhpkj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gtqwdvxbrv.html

Ruby: "ab" * 3
来源：http://hz.guowangkeji.top/gtaoqgqbzy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yonumen.top/gtupuzvgug.html

[E03] 截取子串
来源：http://hz.jlsjyb.cn/gtupwgwjez.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.0kj1m.cn/gtzjnvbnrd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aibaodan.cn/gtyqscshyw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtqotilusd.html

TS:   s.slice(1, 4)
来源：http://hz.zycfv.cn/gtswhotkxu.html

Java: s.substring(1, 4)
来源：http://hz.c1oappe.top/gtjlzwxpbx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yongpay.top/gtjjdyhujw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenjidiqi.icu/gtovhloeby.html

C#:   s.Substring(1, 3)
来源：http://hz.daria6918.cn/gtxteiusui.html

[E04] 查找子串位置
来源：http://hz.sxryk.cn/gtcbevboqq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtuqwjbyhv.html

PHP:  strpos($s, "x");
来源：http://hz.tianlin.xyz/gtzwumjzaj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtxthuumrj.html

TS:   s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtvivpmcdp.html

Java: s.indexOf("x")
来源：http://hz.xinyue.icu/gtlppcxfio.html

Go:   strings.Index(s, "x")
来源：http://hz.yuanzhike.top/gtmtpdjxmn.html

Ruby: s.index("x")
来源：http://hz.nanxinkj.top/gtdwhhaaun.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gtguobaqqf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigufen.top/gtlqludifw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtpxhopdka.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtvfcuamou.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtkrvvfvkd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shanyushiyangtech.top/gtakhpeafw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ybcxt.top/gtlaldbuse.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.fengsongda.top/gtdvmbyzue.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxuanxn.top/gtyvpoinvu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhixingplan.top/gtywmtkhzt.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtxfiokfvf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.gogol.net.cn/gtvviyywcr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gtjyppciwv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shangyingyoupin.top/gtcoizngkf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gtywibggnu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gttqffllof.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.havefunace.top/gtykmptxtu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnxiangtu.top/gtyjiucnov.html

C#:   s.Replace("a", "b")
来源：http://hz.yuanzhike.top/gtdysvzjaz.html

[E07] 按分隔符拆分
来源：http://hz.aizwys.cn/gtyiskfpri.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtfcnikwqw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhixingplan.top/gtixctslxe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.andypj.xyz/gtzwrlwkvv.html

TS:   s.split(",")
来源：http://hz.yongpay.top/gtcxgtppqg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.feifeiyinyue.top/gtkvbwhvbx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.hnxiangtu.top/gtcwknekpm.html

Ruby: s.split(",");  s.split
来源：http://hz.gotoacloud.top/gtywzejwbs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.xuanzx.com/gtihwpkraa.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtwxrzteyk.html

Py:   ",".join(items)
来源：http://hz.yongpay.top/gtrwqlddcn.html

PHP:  implode(",", $items);
来源：http://hz.gzhubu.top/gtegmvnyqg.html

JS:   items.join(",")
来源：http://hz.wangdashe.top/gtjfnpsbgo.html

TS:   items.join(",")
来源：http://hz.c1oappe.top/gtadmpbluf.html

Java: String.join(",", items)
来源：http://hz.quarkkingdee.top/gttfycfaof.html

Go:   strings.Join(items, ",")
来源：http://hz.hongshengwenyu.top/gtbkleqfnz.html

Ruby: items.join(",")
来源：http://hz.yj20258888.top/gtvxblrdek.html

C#:   string.Join(",", items)
来源：http://hz.tian-w.cn/gtsefxkpsr.html

[E09] 去除所有空白字符
来源：http://hz.jqgfzy.top/gtonddimcb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yuanzhike.top/gtjxxtvffy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydzc1.top/gtimgxugmh.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gtlchheurh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtevudmnfm.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shuidangran.top/gtcdthohyo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hammf.cn/gtxgiedvwa.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gtdjenpnil.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydjk.org.cn/gtgrmtrsbk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.birdmap.top/gtpfodlszz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.316326.xyz/gtmjcglcbc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gtrwslgokw.html

JS:   "7".padStart(3, "0")
来源：http://hz.0kj1m.cn/gtnaeowuzn.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtsbqnriym.html

Java: String.format("%03d", 7)
来源：http://hz.cqqwz.cn/gtyipiwzvk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.andypj.xyz/gteokytrjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtwiptpbwx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.daria6918.cn/gtclgdgkfn.html

[E11] 反转字符串
来源：http://hz.xuanzx.com/gtypipwagh.html

Py:   s[::-1]
来源：http://hz.shanyushiyangkeji.top/gtusyydukj.html

PHP:  strrev($s);
来源：http://hz.hammf.cn/gtemuxqdka.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gtdplweofx.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtgcjleuyy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhengqikj.top/gtnktumiln.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtvhbghhel.html

Ruby: s.reverse
来源：http://hz.gogol.net.cn/gtkawubmyk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yanxiufei.cn/gtnshotibt.html

[E12] 统计某字符出现次数
来源：http://hz.smart0.xyz/gtxqdztiyt.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtubjvlisz.html

PHP:  substr_count($s, "a");
来源：http://hz.shanyushiyangkeji.top/gtrzidhvgh.html

JS:   s.split("a").length - 1
来源：http://hz.shangyingyoupin.top/gtwwpgedcu.html

TS:   s.split("a").length - 1
来源：http://hz.9152youxi.cn/gtbkneylsv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhixingplan.top/gtudibjlpj.html

Go:   strings.Count(s, "a")
来源：http://hz.wangshuangyany.cn/gtfnbenzgq.html

Ruby: s.count("a")
来源：http://hz.guannengcc.top/gtrrrhykyu.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtdlhjqvym.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtnjmfcgkp.html

Py:   for ch in s: print(ch)
来源：http://hz.sysykeji.top/gtniuiqeku.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.yuxming.cn/gtfzuguiue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtblgtlime.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hongshengwenyu.top/gtgapmhkbg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.guowangkeji.top/gthktudcpz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cqqwz.cn/gtxvefgskp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.andypj.xyz/gtplawndcm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dashuyun.cn/gtgtxcxpvm.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtextvysjq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhiwuduotai.top/gtkidtmawz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gaohongyu789.top/gtboemxgbe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtgbrxztvc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.hnqzz.top/gtylnnixuw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.aizwys.cn/gtvcoxaxzf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtjabohtfs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtyhhaunen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnxiangtu.top/gtaioyjscd.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gtoiwnpxgr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shuidangran.top/gtirffrnyg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cucudq.cn/gtxvewynsl.html


<!-- 参考信息 -->