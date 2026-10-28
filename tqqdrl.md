代发 wailian999

Java: list.size();
来源：http://hz.jianghu66.top/gtozitmcij.html

Go:   len(arr)
来源：http://hz.cashguo.top/gtodnffflv.html

Ruby: arr.length; arr.size
来源：http://hz.jinqigfzy.top/gtclodwnbz.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtnvkmlhke.html

[D07] 切片 / 取子数组
来源：http://hz.tanke756.top/gtjoqgkeqi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guowangkeji.top/gtzswtacbt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.birdmap.top/gtrcoppmzc.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtaiqbdtab.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigufen.top/gttqoczwuz.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtmrnkrukt.html

Go:   arr[1:4]
来源：http://hz.ivvv.top/gtlvygyvii.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtcspccgql.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgfzy.top/gtixkuaxyk.html

[D08] 合并两个数组
来源：http://hz.zhengqikj.top/gtjuqwnxht.html

Py:   a + b;  a.extend(b)
来源：http://hz.yonumen.top/gtahfhoyhy.html

PHP:  array_merge($a, $b);
来源：http://hz.gotoacloud.top/gtsaetdsdz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.havefunace.top/gtfzjhtnbb.html

TS:   [...a, ...b];
来源：http://hz.yangfankeji.com/gtglgddvmk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zycfv.cn/gthhkxnqmx.html

Go:   append(a, b...)
来源：http://hz.zdqjudy.top/gtyzbhfyam.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hammf.cn/gtqskmotdd.html

C#:   a.Concat(b).ToList()
来源：http://hz.bjfxy.top/gteofsfnxl.html

[D09] 排序（升序）
来源：http://hz.chenzaomai.com/gtebujyjor.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtobiuotld.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtsfcmefjj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtofbljjse.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtuyagglsu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pycfn.com/gttkovnplr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinyuanbaomall.cn/gtdkkfsqdc.html

Ruby: arr.sort
来源：http://hz.shangyingyoupin.top/gtgghoelhp.html

C#:   list.Sort();
来源：http://hz.tanke756.top/gtthrzsvnc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ppjwa.cn/gtzncikicv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtkdnnluzu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtfswphiul.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtdwxwkktx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxinkj.top/gthtdsowhi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtympyuxko.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258888.top/gtuxxnbnkc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.vqdsnc.cn/gtcxhynpbr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.52xcode.cn/gtiplyehol.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtlzayuupt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxuanxn.top/gtnczvwhju.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtttcqgvyh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtdwcfiywk.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtjnycdlat.html

Java: Collections.reverse(list);
来源：http://hz.xingfuxueyuan.xyz/gtzghkqjxq.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258.top/gtzoomivpw.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtkopmotgq.html

C#:   list.Reverse();
来源：http://hz.zdqjudy.top/gtdczumgbp.html

[D12] 查找元素下标
来源：http://hz.ivvv.top/gtnpyavlmp.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtmhuziqcc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ivvv.top/gtnbfmojru.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtpswvvlfl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtgnbyfewo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.guannengcc.top/gtkrkmgwxw.html

Go:   slices.Index(arr, x)
来源：http://hz.tian-w.cn/gtiwlrhlhw.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtrnkmkkbz.html

C#:   list.IndexOf(x);
来源：http://hz.nanxuanxn.top/gtewrophzo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.andypj.xyz/gtiqnsslbc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhaomingkeji.xyz/gtlscgitkg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.vqdsnc.cn/gtroqlugsp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtemqxslzm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.redwolf501.top/gtkkkxqhve.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fengsongda.top/gtbwueacmi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtnjmmdhoq.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gttfrqwvlp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtakyotkof.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cashguo.top/gtiqblburd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jyoumei.cn/gtzzwmmtyq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gtqtgwegbg.html

JS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtgpqrujjf.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtdrfchwsu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gttiaydkjj.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtvplppqzo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenjidiqi.icu/gtssmfoswr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.quarkkingdee.top/gtylkawixi.html

[D15] 去重
来源：http://hz.pycfn.com/gtfadxmhyc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinqigfzy.top/gtbgclrqal.html

PHP:  array_unique($arr);
来源：http://hz.cashguo.top/gtkoylqjwn.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtgtalxhff.html

TS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtbmwcppon.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuetiantiany.cn/gtodgdrwoz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jiagoushi.top/gtwmoecvft.html

Ruby: arr.uniq
来源：http://hz.wangdashe.top/gtasqbypmk.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtkkhgweut.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gteouoelvr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sufxvd.cn/gtvwxrdhva.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cdnleiting.top/gtblpnbjao.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhengqikj.top/gtfcclzqeg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtffscanlm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hnxiangtu.top/gtqncbflxq.html

Go:   // 手写循环累加
来源：http://hz.jqgufenzy.top/gtqndzsvyg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.aizwys.cn/gtgvhvcpnr.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gttyhifjzv.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtzvnmjtaa.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtigvnbruw.html

PHP:  max($arr);  min($arr);
来源：http://hz.yuanzhike.top/gtwoqpppyw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cashguo.top/gtcpjongok.html

TS:   Math.max(...arr);
来源：http://hz.cqqwz.cn/gtyjcllrmt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhengqikj.top/gtvwofmdeb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtoljagssl.html

Ruby: arr.max;  arr.min
来源：http://hz.yanxiufei.cn/gttzzxxgic.html

C#:   list.Max();  list.Min()
来源：http://hz.guannengcc.top/gtuacaxnny.html

[D18] 扁平化嵌套数组
来源：http://hz.fzhhl.top/gtiezyqdtm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shzxlz.cn/gtghknzneq.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtivamsmmr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zdqjudy.top/gtnlnyigte.html

TS:   nested.flat();
来源：http://hz.yuxming.cn/gtmatwapqg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtmdqlpjtp.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtmrvooxyj.html

Ruby: nested.flatten
来源：http://hz.jqgufenzy.top/gtopyrxxdk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yanxiufei.cn/gtuknkikne.html

[D19] 按字段分组
来源：http://hz.ivvv.top/gttvbesrjo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydzc1.top/gtzagrpaep.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jqgfzy.top/gtbvmhibbs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigfzy.top/gtqlwvtzke.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtcdjwfloj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.snrcjt.cn/gtbzmbteez.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtccstjhwo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daria6918.cn/gtbkdycwus.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hnxiangtu.top/gtkfafqciy.html

[D20] 统计每个元素出现次数
来源：http://hz.yonumen.top/gtaotmvjpd.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gthdnppdwg.html

PHP:  array_count_values($arr);
来源：http://hz.sxryk.cn/gtomnthngd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtatdtlvfc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtugwicxfe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhixingplan.top/gtmiwblvja.html

Go:   // 手写 map[T]int
来源：http://hz.daxiang520.top/gtrfgabzvb.html

Ruby: arr.tally
来源：http://hz.redwolf501.top/gtxvenpjgq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.vqdsnc.cn/gtljumapkp.html

[D21] 判断是否包含某元素
来源：http://hz.jlsjyb.cn/gtvtoebgoy.html

Py:   x in arr
来源：http://hz.52xcode.cn/gtznxgfuqz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.svipenyu.cn/gtoqvhkgjd.html

JS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtanjjotsf.html

TS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gtibrazofz.html

Java: list.contains(x)
来源：http://hz.zycfv.cn/gtwywfyjjv.html

Go:   slices.Contains(arr, x)
来源：http://hz.nanxuanxn.top/gtasjmjcjr.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gtvcueqetn.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gtjabrzhrs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hfpthk.cn/gtgfbjdzzt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gtziimpdoa.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yanxiufei.cn/gtiyylgdgx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuxming.cn/gtwuvoqynr.html

TS:   [...arr];
来源：http://hz.daxiang520.top/gtelkuldts.html

Java: new ArrayList<>(list);
来源：http://hz.52xcode.cn/gtxqutyujg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yangfankeji.com/gtbcamxfgz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtbdoztfhx.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtfrvcubue.html

[D23] reduce 累积计算
来源：http://hz.wangdashe.top/gtrtpmbcul.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.316326.xyz/gtxtrrdvsr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fzhhl.top/gtbvlpecnt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtjxbmwuez.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gtsvisozif.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.smart0.xyz/gtwagvovag.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtamziizcg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangshuangyany.cn/gtloamkrgt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.fengsongda.top/gtcpqitbhb.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtrythvhln.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gtbdqcgjdd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtbvcbhjzt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cucudq.cn/gtlyuxkmen.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.c1oappe.top/gtssmffevs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtmuzifcxz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.bjfxy.top/gthrvrvxfb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinghuilouyu.cn/gtiyxblfte.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtkzokpqxb.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtfxryhwjk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xuetiantiany.cn/gtwdptvvsh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gotoacloud.top/gtxwngugsd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtjeqcqlhp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.bjfxy.top/gtixjaojix.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tanke756.top/gtagvobzxa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gaohongyu789.top/gtajgipync.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cqqwz.cn/gtciqqtfll.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.iojbl.cn/gtmgnjyjak.html

[D26] 数组转字符串
来源：http://hz.zhiwuduotai.top/gtxphmcghs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jlsjyb.cn/gtqiafdilu.html

PHP:  implode(", ", $arr);
来源：http://hz.xingfuxueyuan.xyz/gtjxzbikss.html

JS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtzeyrfhxs.html

TS:   arr.join(", ")
来源：http://hz.wangdashe.top/gttgkgilgr.html

Java: String.join(", ", list)
来源：http://hz.zhongyouzk.top/gtxxnoldlv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigufen.top/gtesigsfbs.html

Ruby: arr.join(", ")
来源：http://hz.tian-w.cn/gtjoivkren.html

C#:   string.Join(", ", list)
来源：http://hz.xziqi.cn/gtucpprlec.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtqbfrgxma.html

E. 字符串处理
来源：http://hz.yuanzhike.top/gttbwxomek.html

================================================================================
来源：http://hz.nwbrower.top/gtwklyinfa.html

[E01] 拼接字符串
来源：http://hz.jinghuilouyu.cn/gtgmnieeza.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cucudq.cn/gtujfurysl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dianchejie.cn/gtqicfixmv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtlzqnruwp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhongyouzk.top/gtataxzoif.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dianchejie.cn/gtweqjipgz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.0kj1m.cn/gttxbelrue.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gogol.net.cn/gteiawjhft.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtffxmasup.html

[E02] 重复字符串
来源：http://hz.xziqi.cn/gthxixwwbq.html

Py:   "ab" * 3
来源：http://hz.cashguo.top/gtrmvikojm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gotoacloud.top/gtgnqmfgty.html

JS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtwjuagley.html

TS:   "ab".repeat(3)
来源：http://hz.yanxiufei.cn/gtntaymjhi.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtgdagwyux.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.cqqwz.cn/gtlryazsml.html

Ruby: "ab" * 3
来源：http://hz.fzhhl.top/gtiflqedix.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xuetiantiany.cn/gtleorwzkt.html

[E03] 截取子串
来源：http://hz.jyoumei.cn/gtjmjzohdt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dashuyun.cn/gtanfceqpj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxuanxn.top/gtukmxggvb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtoruodkdc.html

TS:   s.slice(1, 4)
来源：http://hz.hongshengwenyu.top/gtqneewtbv.html

Java: s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtbinyctqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtagfmtufr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtgmscybzb.html

C#:   s.Substring(1, 3)
来源：http://hz.svipenyu.cn/gtdeqvoqya.html

[E04] 查找子串位置
来源：http://hz.vqdsnc.cn/gtixaskiut.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dianchejie.cn/gtpjtkutjr.html

PHP:  strpos($s, "x");
来源：http://hz.hfpthk.cn/gtfqyotips.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhixingplan.top/gturjzplsh.html

TS:   s.indexOf("x")
来源：http://hz.gzhubu.top/gtaitxisri.html

Java: s.indexOf("x")
来源：http://hz.guowangkeji.top/gtrfovvchm.html

Go:   strings.Index(s, "x")
来源：http://hz.feifeiyinyue.top/gtukbqiyqd.html

Ruby: s.index("x")
来源：http://hz.wangdashe.top/gtifuebupv.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtvtuswvou.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtdqezkgut.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.havefunace.top/gtqnzuyalg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hammf.cn/gtwrtswbrh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtuycwmwzt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hfpthk.cn/gtfqcvexta.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtgwhpvwtl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zycfv.cn/gtvpkvsxmb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xylfe.cn/gtbduqdjro.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtgrprpgyf.html

[E06] 替换子串
来源：http://hz.zhixingplan.top/gtxltrkmhb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj202588.top/gtasasrlxu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.0kj1m.cn/gtqupsznhb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtynikdgvi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shanyushiyangtech.top/gtgqstdrbh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jyoumei.cn/gtgjiprgap.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sweek.top/gtipyrlnfi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenzaomai.com/gthamsxacg.html

C#:   s.Replace("a", "b")
来源：http://hz.hfpthk.cn/gtvmpllkmx.html

[E07] 按分隔符拆分
来源：http://hz.ppjwa.cn/gtuxqcebmw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.aibaodan.cn/gtvakpvxzv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtnvdkimrv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.sufxvd.cn/gtvwkrebnv.html

TS:   s.split(",")
来源：http://hz.jinghuilouyu.cn/gtusrdqxgg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuanzx.com/gtgnnajxmm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.9152youxi.cn/gtnxjwsjyn.html

Ruby: s.split(",");  s.split
来源：http://hz.aibaodan.cn/gtpbihgdxv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.snrcjt.cn/gteiosdfek.html

[E08] 数组按分隔符合并
来源：http://hz.cdnleiting.top/gtdxxukqcb.html

Py:   ",".join(items)
来源：http://hz.ehwqpu.com/gtmfhdkuoa.html

PHP:  implode(",", $items);
来源：http://hz.svipenyu.cn/gtvxhsgcdu.html

JS:   items.join(",")
来源：http://hz.guannengcc.top/gtrlyrsbev.html

TS:   items.join(",")
来源：http://hz.xuanzx.com/gtvojkfxvw.html

Java: String.join(",", items)
来源：http://hz.dianchejie.cn/gtnrebcdcb.html

Go:   strings.Join(items, ",")
来源：http://hz.hywenlv.cn/gtqomffmje.html

Ruby: items.join(",")
来源：http://hz.xuanzx.com/gtxtwwxslg.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtpyvrnshw.html

[E09] 去除所有空白字符
来源：http://hz.shangyingyoupin.top/gtbkkdseua.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.iojbl.cn/gtfjkkfdfl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtkoybfcvc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xuanzx.com/gtfkkxwzth.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.guannengcc.top/gtmxotmqtb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yangfankeji.com/gtrvweimxh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtlxgzczke.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hongshengwenyu.top/gtdqlearnb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtdjxurvqx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.bjfxy.top/gtxvyxeqfq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.chenzaomai.com/gtyywyyonc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtffjeualt.html

JS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtmzmoxryh.html

TS:   "7".padStart(3, "0")
来源：http://hz.tanke756.top/gtrqmmzrwp.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtpaehumep.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtvdtsoayc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cdnleiting.top/gtxdemdtsm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhiwuduotai.top/gtqcnueulo.html

[E11] 反转字符串
来源：http://hz.quarkkingdee.top/gtitzotaaf.html

Py:   s[::-1]
来源：http://hz.kuanghao11.cn/gtzbsdsavp.html

PHP:  strrev($s);
来源：http://hz.feifeiyinyue.top/gtnpwhjmdr.html

JS:   [...s].reverse().join("")
来源：http://hz.tianlin.xyz/gtuwqpvqlw.html

TS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtoyjlukvf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhengqikj.top/gtyduiwhqm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sweek.top/gtuniokwsy.html

Ruby: s.reverse
来源：http://hz.xziqi.cn/gtxhlkrcsa.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.andypj.xyz/gtfeiifpia.html

[E12] 统计某字符出现次数
来源：http://hz.fzhhl.top/gtmhcfgfzo.html

Py:   s.count("a")
来源：http://hz.cheryme.top/gtywmwtonx.html

PHP:  substr_count($s, "a");
来源：http://hz.gogol.net.cn/gtmiwryecw.html

JS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gthideuptm.html

TS:   s.split("a").length - 1
来源：http://hz.ydjk.org.cn/gtfychrtss.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.mhx1999.top/gtjdpbabsv.html

Go:   strings.Count(s, "a")
来源：http://hz.pycfn.com/gtswjibcdv.html

Ruby: s.count("a")
来源：http://hz.sweek.top/gttyalgctp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtgdepwjbp.html

[E13] 逐字符遍历
来源：http://hz.cdnleiting.top/gtwnqlbyou.html

Py:   for ch in s: print(ch)
来源：http://hz.smart0.xyz/gtntuheazl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xylfe.cn/gtogsatwmu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuanzx.com/gtlgcgdwmk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtifmojypo.html


<!-- 参考信息 -->