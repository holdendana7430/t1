代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gtefslcmke.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigfzy.top/gtiryrqfmx.html

[D05] 访问与修改元素
来源：http://hz.zycfv.cn/gtrlpktusl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtfqyxhikp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtyjlegwhw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yj20258.top/gtdkqzcajo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhoulong.xyz/gtskoibnyt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aibaodan.cn/gtdljsbagq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtpjpzhblb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtzsyuuvbe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtwlpxsrgt.html

[D06] 数组长度
来源：http://hz.yonumen.top/gtxickpwon.html

Py:   len(arr)
来源：http://hz.snrcjt.cn/gtqywsjrxl.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtefwzeclt.html

JS:   arr.length
来源：http://hz.xinyue.icu/gttywappaz.html

TS:   arr.length
来源：http://hz.yj20258888.top/gtstuofvgj.html

Java: list.size();
来源：http://hz.xingfuxueyuan.xyz/gtmmynzevq.html

Go:   len(arr)
来源：http://hz.wangshuangyany.cn/gtmqjunjjt.html

Ruby: arr.length; arr.size
来源：http://hz.sweek.top/gtprdadxfj.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtuwrykvfl.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtvmmrgngf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.iojbl.cn/gtfqfukhlp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shanyushiyangtech.top/gtikgppjoa.html

JS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gthnggcpxw.html

TS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtjleatgks.html

Java: list.subList(1, 4);
来源：http://hz.hywenlv.cn/gteyqgcoqu.html

Go:   arr[1:4]
来源：http://hz.chenjidiqi.icu/gtvmpmfzwm.html

Ruby: arr[1, 3]
来源：http://hz.cucudq.cn/gtrrjoldbw.html

C#:   list.GetRange(1, 3);
来源：http://hz.jianghu66.top/gtgfpecgir.html

[D08] 合并两个数组
来源：http://hz.gaohongyu789.top/gtnynesunz.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtqgbqmnyj.html

PHP:  array_merge($a, $b);
来源：http://hz.quarkkingdee.top/gtunzonsbf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtyfngmsnj.html

TS:   [...a, ...b];
来源：http://hz.wangdashe.top/gtkpmnihju.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtnrzpdfcy.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gthxgxenue.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtsnvjfzdn.html

C#:   a.Concat(b).ToList()
来源：http://hz.svipenyu.cn/gtwxjqdomu.html

[D09] 排序（升序）
来源：http://hz.ehwqpu.com/gtwdmmxhaj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yvedp.cn/gtfwgetwrb.html

PHP:  sort($arr);
来源：http://hz.cqqwz.cn/gtktbvxvbr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gttnwkgwzr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gtijdhmwpg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtvkyhbegv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtqcchnvgp.html

Ruby: arr.sort
来源：http://hz.c1oappe.top/gtsleviiyf.html

C#:   list.Sort();
来源：http://hz.jqgfzy.top/gtyheslaqe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhiwuduotai.top/gtinabviqb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pengpengdd.cyou/gtpnctrunw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.vqdsnc.cn/gtxnfqejqz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtutvdqhjq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtamcqojct.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.mhx1999.top/gtdortykeh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258888.top/gtcuiblnlf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yonumen.top/gtyzwqwlda.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtfostffcp.html

[D11] 反转数组
来源：http://hz.ywan-chungtsiang.top/gtwvogwhlu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.birdmap.top/gtraylzffk.html

PHP:  array_reverse($arr);
来源：http://hz.yanxiufei.cn/gtqcywrjcn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dianchejie.cn/gtvgpvxbya.html

TS:   [...arr].reverse();
来源：http://hz.iojbl.cn/gtqxflurej.html

Java: Collections.reverse(list);
来源：http://hz.nanxinkj.top/gtynxuelkc.html

Go:   slices.Reverse(arr)
来源：http://hz.sweek.top/gtuugxdowh.html

Ruby: arr.reverse
来源：http://hz.9152youxi.cn/gtsfnokxya.html

C#:   list.Reverse();
来源：http://hz.gaohongyu789.top/gtdwlnwruh.html

[D12] 查找元素下标
来源：http://hz.xinyue.icu/gtqiojvqbt.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtexlkxzyn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.haohaochexian.top/gtlfbjmdxu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtbbfnjxii.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtcazqjrrh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gtfxxuwqom.html

Go:   slices.Index(arr, x)
来源：http://hz.fengsongda.top/gtnwfrcpdh.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangtech.top/gtqhswtgan.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gteivyshpa.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtalhbwnnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.kuanghao11.cn/gtwoxzgslr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.guowangkeji.top/gtcabymrzt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtcshhsdqc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenzaomai.com/gtlgaqlval.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yuxming.cn/gtxwfturbj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtybjyykmp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtrnigojjn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtmmzrnpgz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxuanxn.top/gtqafvnkgu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hongshengwenyu.top/gtlorzipsx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jqgufenzy.top/gthxofqdlf.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtfobdzbip.html

TS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtixyksxae.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtgdvgwhyv.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtxcgjijxl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtgbsgsjek.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenjidiqi.icu/gtgdluqeia.html

[D15] 去重
来源：http://hz.xylfe.cn/gtwjcpeheh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtxnvapibb.html

PHP:  array_unique($arr);
来源：http://hz.jlsjyb.cn/gtmhxcmlep.html

JS:   [...new Set(arr)]
来源：http://hz.pengpengdd.cyou/gtdazaxtsi.html

TS:   [...new Set(arr)]
来源：http://hz.guowangkeji.top/gtrgglwesp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtyqxjoenh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.0kj1m.cn/gtbwopbjdg.html

Ruby: arr.uniq
来源：http://hz.smart0.xyz/gtnjvqzzkt.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtfcdohgmx.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtatouxknk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tianlin.xyz/gtpkajfran.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtxdqchbho.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtygnqehmr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtgeuuowhc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jlsjyb.cn/gtuzcfvbgr.html

Go:   // 手写循环累加
来源：http://hz.ehwqpu.com/gtfyedjxng.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydzc1.top/gtvgtwmrcc.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258.top/gtqisijmwo.html

[D17] 最大值与最小值
来源：http://hz.cqqwz.cn/gtkwaqualh.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtjebvfpjd.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtwxxlytjc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtsaucghtq.html

TS:   Math.max(...arr);
来源：http://hz.meibo888.top/gtskszhhsa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gtqzwrgkgx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtzhggdhce.html

Ruby: arr.max;  arr.min
来源：http://hz.iojbl.cn/gtcubuslog.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtyyhqxbdu.html

[D18] 扁平化嵌套数组
来源：http://hz.0kj1m.cn/gtbmzgobzy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.meibo888.top/gtaqasmzvw.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigufen.top/gtelhmdlds.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.chenzaomai.com/gticwaieyj.html

TS:   nested.flat();
来源：http://hz.tanke756.top/gtxcorgzcq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtcizzxwke.html

Go:   // 手写双层循环
来源：http://hz.meibo888.top/gtsfyjopoc.html

Ruby: nested.flatten
来源：http://hz.hfpthk.cn/gtyjarkswd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtrhhrtnur.html

[D19] 按字段分组
来源：http://hz.cucudq.cn/gtqnusxjuj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fengsongda.top/gtcgauafqr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtywsuejjv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhixingplan.top/gtvlerbiiw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtqoqbnool.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jlsjyb.cn/gttnnwsvbd.html

Go:   // 手写 map[string][]T
来源：http://hz.jlsjyb.cn/gtupzzxsho.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gtonwxpebe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gtluabvrbh.html

[D20] 统计每个元素出现次数
来源：http://hz.ehwqpu.com/gtstffbxxf.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gtyvwpcywh.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtigkwmjxx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtldzkczyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.iojbl.cn/gtnagwjwky.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guannengcc.top/gtnxftksvc.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtalczpuaz.html

Ruby: arr.tally
来源：http://hz.kuanghao11.cn/gtuasuqoua.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gaohongyu789.top/gtqoybdtap.html

[D21] 判断是否包含某元素
来源：http://hz.gotoacloud.top/gteecnrlzu.html

Py:   x in arr
来源：http://hz.svipenyu.cn/gttivlflok.html

PHP:  in_array($x, $arr, true);
来源：http://hz.0kj1m.cn/gtxwfrexxh.html

JS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtyrkcatfa.html

TS:   arr.includes(x)
来源：http://hz.yj20258888.top/gtdjdtvmhi.html

Java: list.contains(x)
来源：http://hz.tianlin.xyz/gtdoyccucl.html

Go:   slices.Contains(arr, x)
来源：http://hz.feifeiyinyue.top/gtbnrnhhco.html

Ruby: arr.include?(x)
来源：http://hz.yvedp.cn/gthcmidnel.html

C#:   list.Contains(x)
来源：http://hz.316326.xyz/gtgntifqrm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.redwolf501.top/gtibntcrfa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydjk.org.cn/gtwifmlcce.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydzc1.top/gtqcthkvnt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zycfv.cn/gtpswavmqk.html

TS:   [...arr];
来源：http://hz.xziqi.cn/gthfxqytev.html

Java: new ArrayList<>(list);
来源：http://hz.gaohongyu789.top/gtsnxyvaag.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cheryme.top/gtjhxolufx.html

Ruby: arr.dup;  arr.clone
来源：http://hz.meibo888.top/gtavktnxod.html

C#:   new List<int>(list);
来源：http://hz.ywan-chungtsiang.top/gtxeseqdmr.html

[D23] reduce 累积计算
来源：http://hz.aibaodan.cn/gtdjlhcsss.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.kuanghao11.cn/gtwtzxuxab.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtgxeernqr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gtbklhfazx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtmoezhjkg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhoulong.xyz/gtruglwfhp.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gttwivssrb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.birdmap.top/gtrgjfjkyd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtppemtpvq.html

[D24] 字典 / Map 基本操作
来源：http://hz.xingfuxueyuan.xyz/gtkhqmihqp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnxiangtu.top/gtvjmcecfv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.svipenyu.cn/gthyothrpz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenjidiqi.icu/gtkbaiksnd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cqqwz.cn/gtphhwtanf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gtomxihlha.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jqgfzy.top/gtwrzgjpjh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gttdaddgqg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtyyuflxnk.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtaadrhkzo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxuanxn.top/gtglcerufr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.havefunace.top/gtedouwske.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jiagoushi.top/gtgbyzulht.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtakdilmzd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydjk.org.cn/gtutjzasyo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtevtrvhoe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gaohongyu789.top/gtgwgbutub.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.iojbl.cn/gtasyptsuh.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtbxvqevei.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xingfuxueyuan.xyz/gtuukmnevc.html

PHP:  implode(", ", $arr);
来源：http://hz.shuidangran.top/gtlwwcetqn.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtbauqcboj.html

TS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtidxziwog.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtrdcoemfa.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydzc1.top/gtyyuglzuz.html

Ruby: arr.join(", ")
来源：http://hz.yj20258888.top/gtmihbkiyh.html

C#:   string.Join(", ", list)
来源：http://hz.quarkkingdee.top/gtkqdawbkl.html

================================================================================
来源：http://hz.hfpthk.cn/gtabvtivku.html

E. 字符串处理
来源：http://hz.jiagoushi.top/gtptcxwunh.html

================================================================================
来源：http://hz.zycfv.cn/gtxgjhsrtt.html

[E01] 拼接字符串
来源：http://hz.zhongyouzk.top/gtwkabgugr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258.top/gtqpsceipo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yanxiufei.cn/gthltlmuxm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtmmkgftxj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtzaqjmxge.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuanzhike.top/gtasbyflbw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gaohongyu789.top/gtmodmnxje.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.316326.xyz/gtfgkfbuud.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gthrwwylrv.html

[E02] 重复字符串
来源：http://hz.fengsongda.top/gtwgydldli.html

Py:   "ab" * 3
来源：http://hz.yvedp.cn/gtflkdwgpx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtatipiaux.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtczmfvkwn.html

TS:   "ab".repeat(3)
来源：http://hz.tian-w.cn/gtlelvqsiq.html

Java: "ab".repeat(3)
来源：http://hz.ybcxt.top/gtxrjzyygp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.0kj1m.cn/gtsditafie.html

Ruby: "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gtcnrlaodl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gtgxiazdgb.html

[E03] 截取子串
来源：http://hz.jinqigfzy.top/gtsxrmsjqg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigfzy.top/gtqkdbtjgq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtucsgsfcx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258.top/gtnelzqytw.html

TS:   s.slice(1, 4)
来源：http://hz.wangshuangyany.cn/gtliimzjjb.html

Java: s.substring(1, 4)
来源：http://hz.316326.xyz/gtossfutnc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtratwbmzk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhengqikj.top/gtognqzaes.html

C#:   s.Substring(1, 3)
来源：http://hz.hywenlv.cn/gthlermzvc.html

[E04] 查找子串位置
来源：http://hz.jqgfzy.top/gtopbsbiqr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhongyouzk.top/gtczqoxyfs.html

PHP:  strpos($s, "x");
来源：http://hz.havefunace.top/gtjohyalqb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.birdmap.top/gtxtnazgin.html

TS:   s.indexOf("x")
来源：http://hz.jinqigfzy.top/gtbjjbmtbr.html

Java: s.indexOf("x")
来源：http://hz.jqgufenzy.top/gtehpbbpbh.html

Go:   strings.Index(s, "x")
来源：http://hz.yongpay.top/gtfhyjjigd.html

Ruby: s.index("x")
来源：http://hz.shzxlz.cn/gtczkzcpps.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtfntwvzls.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtspfbxiqq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shzxlz.cn/gtoldgjnle.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gtqramiuyh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.316326.xyz/gtoqhccilu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yj20258888.top/gturskugtw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinghuilouyu.cn/gtqukgipjp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cqqwz.cn/gtljzjufvp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gogol.net.cn/gttuewxkho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.9152youxi.cn/gtnhwbenxs.html

[E06] 替换子串
来源：http://hz.tianlin.xyz/gtjsuhmqql.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.iojbl.cn/gtnuuvkfst.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.bjfxy.top/gtrwcsokxd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.nanxinkj.top/gtytkwglne.html

TS:   s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtvypbecsw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.c1oappe.top/gtzmohvmhz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.dashuyun.cn/gtqdmxnmkc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.redwolf501.top/gtiwyhnblx.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtzraletay.html

[E07] 按分隔符拆分
来源：http://hz.iojbl.cn/gtmzxvnoce.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnxiangtu.top/gtsrirsnjz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.birdmap.top/gtclpklfin.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtfajrfmap.html

TS:   s.split(",")
来源：http://hz.jiagoushi.top/gtwlnajzzl.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhongyouzk.top/gtfhpdhjsq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtryonrxuj.html

Ruby: s.split(",");  s.split
来源：http://hz.ywan-chungtsiang.top/gtpcodjzwx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sufxvd.cn/gtneanszyb.html

[E08] 数组按分隔符合并
来源：http://hz.chenzaomai.com/gtizdekohq.html

Py:   ",".join(items)
来源：http://hz.xingfuxueyuan.xyz/gtrgihdqjj.html

PHP:  implode(",", $items);
来源：http://hz.xuanzx.com/gtdmnnwhav.html

JS:   items.join(",")
来源：http://hz.hywenlv.cn/gtmjbtvidv.html

TS:   items.join(",")
来源：http://hz.snrcjt.cn/gtojbztvjb.html

Java: String.join(",", items)
来源：http://hz.hnqzz.top/gtopqugmvt.html

Go:   strings.Join(items, ",")
来源：http://hz.gogol.net.cn/gttebaswca.html

Ruby: items.join(",")
来源：http://hz.jinqigufen.top/gtqmshptgt.html

C#:   string.Join(",", items)
来源：http://hz.sweek.top/gthwbpxcuz.html

[E09] 去除所有空白字符
来源：http://hz.bjfxy.top/gtdrejpdja.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhengqikj.top/gtckwhvlbr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangdashe.top/gtezqjvzai.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtqwzvtbha.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinghuilouyu.cn/gtytyrtlsl.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.feifeiyinyue.top/gtdsbhcbre.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gtfrwurhay.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangshuangyany.cn/gtjeuzsdhp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yongpay.top/gtqebqhzfl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.nwbrower.top/gtbanqqjyo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nwbrower.top/gtmzgfjbvn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.wangshuangyany.cn/gtbjtoihno.html

JS:   "7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtedjtktyx.html

TS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtryibarvy.html

Java: String.format("%03d", 7)
来源：http://hz.shanyushiyangtech.top/gtjtdwicsc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtbpbzqfal.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtvvyjhbud.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.fengsongda.top/gtldrjjktg.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtgpqtfhxy.html

Py:   s[::-1]
来源：http://hz.sysykeji.top/gtouxwtqca.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gthepxswim.html

JS:   [...s].reverse().join("")
来源：http://hz.havefunace.top/gttfztggpp.html

TS:   [...s].reverse().join("")
来源：http://hz.yongpay.top/gtxbutzfhp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gotoacloud.top/gtsxuhaapd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yonumen.top/gtmnggkkzx.html


<!-- 参考信息 -->