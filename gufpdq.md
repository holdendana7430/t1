代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.xziqi.cn/gtxypmhwrn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cucudq.cn/gtzlyybbmx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.guannengcc.top/gtiyosjzdi.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtvulgvaud.html

TS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtwrxxbhqn.html

Java: list.subList(1, 4);
来源：http://hz.haohaochexian.top/gtttlgovik.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gtvbirpybh.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gthfbpjptj.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangdashe.top/gtwrmhpvfw.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtejhfjuva.html

Py:   a + b;  a.extend(b)
来源：http://hz.ywan-chungtsiang.top/gtyrxtvebj.html

PHP:  array_merge($a, $b);
来源：http://hz.hnxiangtu.top/gtytbnvedm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.feifeiyinyue.top/gtyhyqtnwf.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtxmsnzgpc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.vqdsnc.cn/gtdhscyivb.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtysatpjlf.html

Ruby: a + b;  a.concat(b)
来源：http://hz.mhx1999.top/gtbkeeyddx.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtepbxsgvf.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtekyhwtue.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenjidiqi.icu/gtfcoefdzu.html

PHP:  sort($arr);
来源：http://hz.smart0.xyz/gtldorrdiv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hfpthk.cn/gtcuesndim.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tanke756.top/gtrbkdxkou.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yueranfly.top/gtjtbrjwwf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtaulwfiys.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtxjazwrnv.html

C#:   list.Sort();
来源：http://hz.jqgufenzy.top/gtubsmefiq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtsclyiowg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.haohaochexian.top/gtjrgejfua.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xylfe.cn/gttaziqxug.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gttjxdasvk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jlsjyb.cn/gtylzrquzu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ivvv.top/gtlyumlyqn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cdnleiting.top/gtuxajjzpr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgfzy.top/gtmlgoldba.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fzhhl.top/gttaymyurn.html

[D11] 反转数组
来源：http://hz.iojbl.cn/gtikwmddok.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gthlglbbyb.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gthwjmlhpm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hnqzz.top/gtuzgoiafr.html

TS:   [...arr].reverse();
来源：http://hz.daxiang520.top/gtqdmpwjbm.html

Java: Collections.reverse(list);
来源：http://hz.gaohongyu789.top/gtlhcjfihg.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gteyszcqvq.html

Ruby: arr.reverse
来源：http://hz.pycfn.com/gtxkgnxzve.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtntigfean.html

[D12] 查找元素下标
来源：http://hz.haohaochexian.top/gtuxdiwfsi.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gtllirbieg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yanxiufei.cn/gtcfvfyiba.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtquawfdfr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtrnovvrcr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.meibo888.top/gtoiorsipv.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gthcafjnro.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gtruzokggl.html

C#:   list.IndexOf(x);
来源：http://hz.ivvv.top/gtofbtmubg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangshuangyany.cn/gtfimphfqd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtrlvkjeik.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gthekwvphb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtpxekvkiu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.birdmap.top/gtowamzlqa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhoulong.xyz/gtdowbdvnj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtklmifuyf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zycfv.cn/gtnqeeutyo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sufxvd.cn/gtcnrlffzx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtlggmzcqq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xylfe.cn/gtynogkyjv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtryaxdesg.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtkopzufnd.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtnwllpnnt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtemlubydq.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtkklkavmn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenlongwang.top/gtommifwdi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.mhx1999.top/gtujsgglle.html

[D15] 去重
来源：http://hz.mhx1999.top/gtezxnqhmf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtruzldzpe.html

PHP:  array_unique($arr);
来源：http://hz.hammf.cn/gtfhcznaab.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gttowqiqhb.html

TS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtwjqtggqa.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhoulong.xyz/gtjiaimpnn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cdnleiting.top/gtjegpgril.html

Ruby: arr.uniq
来源：http://hz.xziqi.cn/gtpbfrrhmn.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258888.top/gtmgowoumx.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtexpzfkeh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtsmqvtnqc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhiwuduotai.top/gtokpsvzac.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtuuvjoykt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cheryme.top/gtlqoijads.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhongyouzk.top/gtvmsqxlay.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtbhfqsjqz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yangfankeji.com/gtjwxykltk.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtljfyqwzy.html

[D17] 最大值与最小值
来源：http://hz.andypj.xyz/gtfxlpzdec.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtqjmfmpql.html

PHP:  max($arr);  min($arr);
来源：http://hz.havefunace.top/gtjmwdfpit.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangshuangyany.cn/gtvqhfwdzr.html

TS:   Math.max(...arr);
来源：http://hz.52xcode.cn/gtgttifsmi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yonumen.top/gtyiybajtd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.daria6918.cn/gtwwdsqaes.html

Ruby: arr.max;  arr.min
来源：http://hz.cucudq.cn/gtmpnbsxqr.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxuanxn.top/gtqxjwjfib.html

[D18] 扁平化嵌套数组
来源：http://hz.cashguo.top/gtsrosgvbu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtjnsloqjk.html

PHP:  array_merge(...$nested);
来源：http://hz.zhixingplan.top/gtzytbrbec.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.svipenyu.cn/gtbvkcbhzm.html

TS:   nested.flat();
来源：http://hz.jinghuilouyu.cn/gtxeijzypy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenzaomai.com/gtujenejqf.html

Go:   // 手写双层循环
来源：http://hz.wangdashe.top/gtyldlswft.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtopiwyqpb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtpfhkjbvb.html

[D19] 按字段分组
来源：http://hz.ppjwa.cn/gtoigtywcb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yanxiufei.cn/gtdnuziyor.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pengpengdd.cyou/gtlpxiyeeg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtydnlcdls.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtygfcyygv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtydvvfzzn.html

Go:   // 手写 map[string][]T
来源：http://hz.cheryme.top/gtqhjdutvn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtqzihbjlu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pengpengdd.cyou/gtfmggaroj.html

[D20] 统计每个元素出现次数
来源：http://hz.daria6918.cn/gtwkbjmvoo.html

Py:   Counter(arr)
来源：http://hz.shanyushiyangtech.top/gtauwsixfm.html

PHP:  array_count_values($arr);
来源：http://hz.xylfe.cn/gtmgeflomu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtkiwbfjbs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtqqwtvooc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pycfn.com/gttyjsopcy.html

Go:   // 手写 map[T]int
来源：http://hz.redwolf501.top/gtfqbeyibl.html

Ruby: arr.tally
来源：http://hz.tian-w.cn/gtdqjszlls.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhongyouzk.top/gtfcxzdaqh.html

[D21] 判断是否包含某元素
来源：http://hz.snrcjt.cn/gtluntxgpb.html

Py:   x in arr
来源：http://hz.yj20258888.top/gtnspbfxdk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinqigfzy.top/gtwjpszbph.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtunyqrwel.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtkcbvzhgm.html

Java: list.contains(x)
来源：http://hz.dianchejie.cn/gthnnnmhft.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhongyouzk.top/gtqiyxdlem.html

Ruby: arr.include?(x)
来源：http://hz.sxryk.cn/gtiopakvbw.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtzgsrdyeu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zdqjudy.top/gthjxjkjvq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.dashuyun.cn/gtnxdzgjlm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jlsjyb.cn/gthkrlscau.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.mhx1999.top/gtazftthty.html

TS:   [...arr];
来源：http://hz.ywan-chungtsiang.top/gtmmefanee.html

Java: new ArrayList<>(list);
来源：http://hz.chenjidiqi.icu/gtrbpzkpnd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.quarkkingdee.top/gtmjyigtgn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtovtdgiqy.html

C#:   new List<int>(list);
来源：http://hz.xziqi.cn/gtiqzqjvvm.html

[D23] reduce 累积计算
来源：http://hz.ivvv.top/gtiyimgfak.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuanzx.com/gtuxymomir.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aibaodan.cn/gtihebgxxi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gttjzpxlxe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtvvjvisjv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhoulong.xyz/gtuksujwjk.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtirclpcft.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fengsongda.top/gtohkmbwyk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gtovybtprp.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtlleucqco.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xingfuxueyuan.xyz/gtkhaxozjf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtarsjxxkm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtqbraasmv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.shuidangran.top/gtxmstfmyw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fzhhl.top/gtkncrljta.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtrdxkefnt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gtwhvkqesi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.andypj.xyz/gtgsovwzxc.html

[D25] Set 集合去重与交并差
来源：http://hz.aizwys.cn/gtbhdtjqta.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangtech.top/gtghgrwyzg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtyeguozhl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtmbnxwoxw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.0kj1m.cn/gtpokrrlzj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jqgfzy.top/gtrsnlzhof.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhengqikj.top/gthnzdnhsa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtnzxikoxo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zdqjudy.top/gtwztcfptu.html

[D26] 数组转字符串
来源：http://hz.yongpay.top/gtknmoshci.html

Py:   ", ".join(map(str, arr))
来源：http://hz.fengsongda.top/gtlhfjjkrd.html

PHP:  implode(", ", $arr);
来源：http://hz.gaohongyu789.top/gtbrzoncxv.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtsgqdyzeb.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtpmxwtprn.html

Java: String.join(", ", list)
来源：http://hz.svipenyu.cn/gtzkvdvkur.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gtddnbgmdo.html

Ruby: arr.join(", ")
来源：http://hz.dianchejie.cn/gtqdvwhxgs.html

C#:   string.Join(", ", list)
来源：http://hz.shuidangran.top/gthinhtmgf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtenksxtfo.html

E. 字符串处理
来源：http://hz.xingfuxueyuan.xyz/gttnhfnwta.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqdyrphsf.html

[E01] 拼接字符串
来源：http://hz.xingfuxueyuan.xyz/gtpwwjbzjl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.52xcode.cn/gttuotmfwp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gtoamoxtdy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtkhagknrv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258888.top/gtomzelpmm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yueranfly.top/gtybyhnhlf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuanzhike.top/gtkrzznxmm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinghuilouyu.cn/gthrjzghrv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bjfxy.top/gtfzbbupya.html

[E02] 重复字符串
来源：http://hz.zhongyouzk.top/gtxepirhwj.html

Py:   "ab" * 3
来源：http://hz.sysykeji.top/gtktjwycta.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinghuilouyu.cn/gtwvbyqbcc.html

JS:   "ab".repeat(3)
来源：http://hz.chenjidiqi.icu/gtfmkkedwl.html

TS:   "ab".repeat(3)
来源：http://hz.xylfe.cn/gtebjmjzow.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtjpeczakd.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.bjfxy.top/gthvczkqjw.html

Ruby: "ab" * 3
来源：http://hz.xingfuxueyuan.xyz/gtpkspekxp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.svipenyu.cn/gtcdmcnyln.html

[E03] 截取子串
来源：http://hz.sufxvd.cn/gtqhipqwmw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangshuangyany.cn/gtrksokpqe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zycfv.cn/gtxksjtijy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtgimoyomx.html

TS:   s.slice(1, 4)
来源：http://hz.jlsjyb.cn/gtrtmcjutk.html

Java: s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtexhdjdjg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yvedp.cn/gtrsfgiljt.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ehwqpu.com/gtzyqvfxnw.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtigdagprl.html

[E04] 查找子串位置
来源：http://hz.zhixingplan.top/gtofddnmdh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtjlqnvdfu.html

PHP:  strpos($s, "x");
来源：http://hz.smart0.xyz/gtehbakmjy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtcemfepvr.html

TS:   s.indexOf("x")
来源：http://hz.gzhubu.top/gtzyguqnhn.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtlksavfxi.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gtvougzarr.html

Ruby: s.index("x")
来源：http://hz.316326.xyz/gteyrtehkq.html

C#:   s.IndexOf("x")
来源：http://hz.sysykeji.top/gtzbivpwfx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtrolomgqz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.c1oappe.top/gtchxyxqau.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.aibaodan.cn/gtyycrzkof.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtxurkaugg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhongyouzk.top/gtxilpchri.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtgavzxpye.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.chenjidiqi.icu/gtmadxulvj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nwbrower.top/gtiacqkmvs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgfzy.top/gtalecyfmt.html

[E06] 替换子串
来源：http://hz.9152youxi.cn/gtosvxxqrn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cdnleiting.top/gtmpjoxtfp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtfxsiimgk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtzxufbiyi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtdoinqeqm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtkzedodgi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yj20258888.top/gtinjryhwz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.c1oappe.top/gtkcjqxirf.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtgsyibavp.html

[E07] 按分隔符拆分
来源：http://hz.52xcode.cn/gttgzzypzq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jinqigfzy.top/gtvuzafyxk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigfzy.top/gthhwyukdo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.chenzaomai.com/gtcwlhpoyn.html

TS:   s.split(",")
来源：http://hz.yonumen.top/gtmsniktik.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xuetiantiany.cn/gteefmhlpg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.pengpengdd.cyou/gthpjzjerv.html

Ruby: s.split(",");  s.split
来源：http://hz.9152youxi.cn/gtffniwazf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yongpay.top/gtssnyeoep.html

[E08] 数组按分隔符合并
来源：http://hz.jianghu66.top/gtjwotkkcg.html

Py:   ",".join(items)
来源：http://hz.zhongyouzk.top/gtepobrszy.html

PHP:  implode(",", $items);
来源：http://hz.cucudq.cn/gtyuxfudvi.html

JS:   items.join(",")
来源：http://hz.mhx1999.top/gtrvyozmzw.html

TS:   items.join(",")
来源：http://hz.xuetiantiany.cn/gtezarozil.html

Java: String.join(",", items)
来源：http://hz.cucudq.cn/gtcmsbmtyj.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtfyjuoffx.html

Ruby: items.join(",")
来源：http://hz.jianghu66.top/gtduengbql.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gtnpydyrxt.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gtupghrzaj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.daxiang520.top/gtyhsbpivm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jyoumei.cn/gtfeqnxrnt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtstniuhgg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtxchvjnvh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.316326.xyz/gtnghdtoqg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gtqcxollke.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dianchejie.cn/gthjgrdbue.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yvedp.cn/gtaltddtfy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.c1oappe.top/gtsqzbpmez.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.iojbl.cn/gtxdcfisly.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tanke756.top/gtzqkbczas.html

JS:   "7".padStart(3, "0")
来源：http://hz.xylfe.cn/gtpjvpnayb.html

TS:   "7".padStart(3, "0")
来源：http://hz.ydzc1.top/gtdqwgxacu.html

Java: String.format("%03d", 7)
来源：http://hz.feifeiyinyue.top/gtxzwquwpl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.aizwys.cn/gtdzwfaalo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.smart0.xyz/gtmnihzyrz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yanxiufei.cn/gtwayqgoqq.html

[E11] 反转字符串
来源：http://hz.xinyue.icu/gtlbjpritp.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gthcefovsg.html

PHP:  strrev($s);
来源：http://hz.tanke756.top/gtlpuvlqcy.html

JS:   [...s].reverse().join("")
来源：http://hz.yonumen.top/gtuiolphmi.html

TS:   [...s].reverse().join("")
来源：http://hz.hywenlv.cn/gtgcgdmwyh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xuanzx.com/gteurbqfns.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtukjhvhux.html

Ruby: s.reverse
来源：http://hz.shangyingyoupin.top/gtegdwytjr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shzxlz.cn/gtbjvqmual.html

[E12] 统计某字符出现次数
来源：http://hz.ydzc1.top/gttugtvaff.html

Py:   s.count("a")
来源：http://hz.jinqigfzy.top/gtrnoejyob.html

PHP:  substr_count($s, "a");
来源：http://hz.bjfxy.top/gtsejvmmgs.html

JS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtrtfgvbhh.html

TS:   s.split("a").length - 1
来源：http://hz.andypj.xyz/gtsmokqvsx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yvedp.cn/gtkpusxacm.html

Go:   strings.Count(s, "a")
来源：http://hz.redwolf501.top/gteoldypnj.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtlqwtfaen.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yanxiufei.cn/gtnkwqszmf.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtijognunf.html

Py:   for ch in s: print(ch)
来源：http://hz.wangdashe.top/gtvnkzvbka.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.aibaodan.cn/gtustzjumk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtvzmtmese.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258.top/gtqkcelbnl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yongpay.top/gtywofbpgj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shanyushiyangtech.top/gtqyukjzbv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.316326.xyz/gtzustqrbz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ivvv.top/gtglzwqtor.html


<!-- 参考信息 -->