代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtbdufbkcm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhoulong.xyz/gtvvjdvhvw.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtsdbofrls.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gttqcfzyzi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.haohaochexian.top/gtycqbgrau.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydzc1.top/gtxncfatsc.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guowangkeji.top/gtxvehkoar.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tanke756.top/gtoyxwbyrt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xylfe.cn/gtqcdrcllw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nwbrower.top/gtehmgvyad.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtsmyumosw.html

[D06] 数组长度
来源：http://hz.cashguo.top/gtauapgdjb.html

Py:   len(arr)
来源：http://hz.zhixingplan.top/gtyfjzkdhv.html

PHP:  count($arr);
来源：http://hz.dianchejie.cn/gtfqpkrdyu.html

JS:   arr.length
来源：http://hz.zhijiandao.cn/gtfsayepuc.html

TS:   arr.length
来源：http://hz.quarkkingdee.top/gtrdqimupk.html

Java: list.size();
来源：http://hz.sufxvd.cn/gtoiygiqtt.html

Go:   len(arr)
来源：http://hz.yuanzhike.top/gtyccvfmdd.html

Ruby: arr.length; arr.size
来源：http://hz.haohaochexian.top/gtvsquompt.html

C#:   list.Count;
来源：http://hz.zycfv.cn/gtgsebfted.html

[D07] 切片 / 取子数组
来源：http://hz.yongpay.top/gtkcnmzcaq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ppjwa.cn/gtmzrvlmpk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.bjfxy.top/gtpojmfmby.html

JS:   arr.slice(1, 4);
来源：http://hz.cashguo.top/gtizxrqkjr.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtvjrvnhws.html

Java: list.subList(1, 4);
来源：http://hz.aizwys.cn/gtormswjjd.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtgabsmedw.html

Ruby: arr[1, 3]
来源：http://hz.pengpengdd.cyou/gthgsfcqvn.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigfzy.top/gtnheziagz.html

[D08] 合并两个数组
来源：http://hz.jiagoushi.top/gtxyxwgxnp.html

Py:   a + b;  a.extend(b)
来源：http://hz.tanke756.top/gtzyrmloqw.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxinkj.top/gtigijqhfq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtaepsrueh.html

TS:   [...a, ...b];
来源：http://hz.sysykeji.top/gtacrsdxgk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hammf.cn/gtosuxwyzg.html

Go:   append(a, b...)
来源：http://hz.hfpthk.cn/gtcguodrjy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yvedp.cn/gtpaofxgbi.html

C#:   a.Concat(b).ToList()
来源：http://hz.0kj1m.cn/gtvwjhzwvl.html

[D09] 排序（升序）
来源：http://hz.316326.xyz/gtdmitfdti.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtijfpwukg.html

PHP:  sort($arr);
来源：http://hz.cqqwz.cn/gtodsynyye.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gttjccpjir.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinghuilouyu.cn/gtyayeavtx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinghuilouyu.cn/gtbjyqvied.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtcrdqzkfv.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gttzhfqnkk.html

C#:   list.Sort();
来源：http://hz.c1oappe.top/gtmfotemch.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nanxuanxn.top/gtugimiuck.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtigvlidof.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangshuangyany.cn/gtmrvalolp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtaiuqydvb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydjk.org.cn/gtmdwreugd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gtmwvrtmqt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangtech.top/gtdnpeqvdr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jlsjyb.cn/gttmagdtdg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gtxopfksuj.html

[D11] 反转数组
来源：http://hz.smart0.xyz/gtjfxvbzyg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtowggkhyz.html

PHP:  array_reverse($arr);
来源：http://hz.gotoacloud.top/gtrgbzlveu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gtqqzijujp.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtvvhhgrzw.html

Java: Collections.reverse(list);
来源：http://hz.iojbl.cn/gtykfqrtui.html

Go:   slices.Reverse(arr)
来源：http://hz.cashguo.top/gtepbzyvjq.html

Ruby: arr.reverse
来源：http://hz.vqdsnc.cn/gtxmbyolek.html

C#:   list.Reverse();
来源：http://hz.hnqzz.top/gtylaffoxs.html

[D12] 查找元素下标
来源：http://hz.shangyingyoupin.top/gtgtvynycn.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhongyouzk.top/gthznsxtmf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtqmdupkux.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gtpnjasdlb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtzsynguyc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pengpengdd.cyou/gtcuwwxvjs.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtfugdavmg.html

Ruby: arr.index(x)
来源：http://hz.chenlongwang.top/gtpwhnweec.html

C#:   list.IndexOf(x);
来源：http://hz.zhiwuduotai.top/gtjbsnelau.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinyuanbaomall.cn/gtjpzmssgv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinyuanbaomall.cn/gtwjshpigc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gthvawmweg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.chenjidiqi.icu/gtpzfhrroz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtsrcpxtdk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.meibo888.top/gtgyeqscwf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtybevmpkw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnxiangtu.top/gtjrsxrjfn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtxjggduep.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtpbdqhhlq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.havefunace.top/gtifhmzrfe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gtgoeclqfv.html

JS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtkkzpwsre.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtrqevikel.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinghuilouyu.cn/gtnltnlpbn.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtppqyptdl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gthpludonn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtqxahjwmj.html

[D15] 去重
来源：http://hz.316326.xyz/gtumzylssy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtslbxzofb.html

PHP:  array_unique($arr);
来源：http://hz.jinqigufen.top/gtgpqniixj.html

JS:   [...new Set(arr)]
来源：http://hz.jinqigufen.top/gtmjcmlnnt.html

TS:   [...new Set(arr)]
来源：http://hz.shangyingyoupin.top/gtirlcgpcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtbbqahhpk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtvdlzfzxd.html

Ruby: arr.uniq
来源：http://hz.zhengqikj.top/gtaymbtkmf.html

C#:   list.Distinct().ToList()
来源：http://hz.ydjk.org.cn/gtyzhzcbof.html

[D16] 求和与平均值
来源：http://hz.ivvv.top/gtzmhdcoav.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dianchejie.cn/gtxnziljzo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ivvv.top/gtfgihglni.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtphizypwk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtcoihtkvc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhixingplan.top/gtfwzhefbh.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtxsauvbjj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gtebpcgmik.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtakshfpib.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gthdkafgve.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtkuwwbiqc.html

PHP:  max($arr);  min($arr);
来源：http://hz.quarkkingdee.top/gtulijcygj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cheryme.top/gtruhkbfkh.html

TS:   Math.max(...arr);
来源：http://hz.ywan-chungtsiang.top/gtaksltjar.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxuanxn.top/gtxazxmiyo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zycfv.cn/gtsqzspcbf.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtwmiaxozv.html

C#:   list.Max();  list.Min()
来源：http://hz.aizwys.cn/gtwtrdybyl.html

[D18] 扁平化嵌套数组
来源：http://hz.yonumen.top/gtvrwpxcnj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydjk.org.cn/gtugydqrod.html

PHP:  array_merge(...$nested);
来源：http://hz.shanyushiyangkeji.top/gtoqotqxjx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtwdzljuqf.html

TS:   nested.flat();
来源：http://hz.0kj1m.cn/gteozxrmio.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cheryme.top/gtkdvafati.html

Go:   // 手写双层循环
来源：http://hz.zycfv.cn/gtaxhmhbrv.html

Ruby: nested.flatten
来源：http://hz.tanke756.top/gtxihgthit.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ppjwa.cn/gttrgxnecq.html

[D19] 按字段分组
来源：http://hz.cheryme.top/gtqnqaypxm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gtoshwdifc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinyuanbaomall.cn/gtdrhbskcm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtfujsread.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sufxvd.cn/gtercporxg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dianchejie.cn/gtugfyfryr.html

Go:   // 手写 map[string][]T
来源：http://hz.mhx1999.top/gtrgjmxcub.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.quarkkingdee.top/gtcfteguim.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinyuanbaomall.cn/gtlfxqgibg.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gturrmrkfy.html

Py:   Counter(arr)
来源：http://hz.haohaochexian.top/gthwelweol.html

PHP:  array_count_values($arr);
来源：http://hz.wangdashe.top/gtsddhebzx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtspwaabyd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtacvshxqi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jinyuanbaomall.cn/gtnyimlkjh.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigufen.top/gtqshjvuef.html

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtcmfgdash.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hysaishi.cn/gtwngzdgzz.html

[D21] 判断是否包含某元素
来源：http://hz.cdnleiting.top/gtsgkurwpl.html

Py:   x in arr
来源：http://hz.c1oappe.top/gtbivtqtir.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cashguo.top/gtmiqnzgfd.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtpqeofvid.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtajayrhva.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtjqiqoqzf.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigfzy.top/gtfdyozxmk.html

Ruby: arr.include?(x)
来源：http://hz.sxryk.cn/gtivyspqas.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtshsytfip.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigfzy.top/gtzkjncihw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.quarkkingdee.top/gtxaptkxtp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtqkplwuli.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guowangkeji.top/gtrvntjuuf.html

TS:   [...arr];
来源：http://hz.hywenlv.cn/gtvjrvzugb.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtqtvicnkf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.redwolf501.top/gtqzuoyrfk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ydjk.org.cn/gtikuqsrnq.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtolaeezxj.html

[D23] reduce 累积计算
来源：http://hz.zhoulong.xyz/gtvjywujty.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangshuangyany.cn/gtiflgxzqe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zdqjudy.top/gtrxeemvys.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtehqzizvo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtwldkwhza.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtiiszdtzs.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtxcchatzq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gtepbykxdp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258.top/gtofqozpva.html

[D24] 字典 / Map 基本操作
来源：http://hz.hongshengwenyu.top/gtzszetlwr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtselwnila.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nanxuanxn.top/gtaoqnhnyz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtnclvjwgx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cqqwz.cn/gtohvxynqa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jiagoushi.top/gtwifvdbpa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yangfankeji.com/gtyltddtus.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gzhubu.top/gtfxwleszr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jlsjyb.cn/gtnfozkkzm.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtpryaobix.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtnusstnjl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtajhohuyh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hammf.cn/gttexsrgkw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shangyingyoupin.top/gtgldlygbb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj202588.top/gtleiezjto.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangdashe.top/gtpcqfxkye.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jyoumei.cn/gtijycrcma.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtfqfvvpky.html

[D26] 数组转字符串
来源：http://hz.cheryme.top/gtezxjjeaq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ppjwa.cn/gtsboaueop.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gtwcvjbwzm.html

JS:   arr.join(", ")
来源：http://hz.yj20258.top/gtmwkponfz.html

TS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtnfajhfyr.html

Java: String.join(", ", list)
来源：http://hz.cucudq.cn/gtcemzkttc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuanzx.com/gtzxlwgimo.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtekasylsw.html

C#:   string.Join(", ", list)
来源：http://hz.xinyue.icu/gttmxxcgcp.html

================================================================================
来源：http://hz.jyoumei.cn/gtzwpkooii.html

E. 字符串处理
来源：http://hz.shuidangran.top/gtekurclpn.html

================================================================================
来源：http://hz.ydzc1.top/gtlekwwaxq.html

[E01] 拼接字符串
来源：http://hz.jinghuilouyu.cn/gtprqfxpib.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.bjfxy.top/gtolexrdqn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtjjceyqbn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtnrfefeob.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnqzz.top/gtogynjdhj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.havefunace.top/gtchlzezjw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jinghuilouyu.cn/gtkvprunhy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gtzaxklymq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.nanxuanxn.top/gtomlmnzgy.html

[E02] 重复字符串
来源：http://hz.nwbrower.top/gtvghixeul.html

Py:   "ab" * 3
来源：http://hz.cqqwz.cn/gtadrlvjgw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.gaohongyu789.top/gthwoiqvqu.html

JS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtndtbftya.html

TS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtlmduhfqv.html

Java: "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtnddlkqpt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtyddwryky.html

Ruby: "ab" * 3
来源：http://hz.hfpthk.cn/gthdmadszb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yongpay.top/gtmjyonobh.html

[E03] 截取子串
来源：http://hz.wangshuangyany.cn/gtkrxbmzfz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ppjwa.cn/gtdsrurhgc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.316326.xyz/gtijqnzrpy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj202588.top/gtsqtsyctn.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gthqjhxrhw.html

Java: s.substring(1, 4)
来源：http://hz.shzxlz.cn/gtewwpyyqz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pycfn.com/gtukkzshyw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtevalwdlu.html

C#:   s.Substring(1, 3)
来源：http://hz.ywan-chungtsiang.top/gtuqbhcjsl.html

[E04] 查找子串位置
来源：http://hz.zhengqikj.top/gtmtqriazi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yueranfly.top/gtvskwyoiw.html

PHP:  strpos($s, "x");
来源：http://hz.haohaochexian.top/gtwzminnfk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.redwolf501.top/gtfynxhmyu.html

TS:   s.indexOf("x")
来源：http://hz.wangdashe.top/gtzpgreiej.html

Java: s.indexOf("x")
来源：http://hz.yonumen.top/gtrdigkrod.html

Go:   strings.Index(s, "x")
来源：http://hz.sysykeji.top/gtckbzvgzi.html

Ruby: s.index("x")
来源：http://hz.sufxvd.cn/gtatgnyira.html

C#:   s.IndexOf("x")
来源：http://hz.havefunace.top/gtrqhjtrdk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtqwybgium.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.quarkkingdee.top/gtkeiahaxw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.9152youxi.cn/gtorvptpaj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtoxtjiibr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hysaishi.cn/gtjpdujvio.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinyuanbaomall.cn/gtvvyyzdxa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shuidangran.top/gtrrdjlitg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.smart0.xyz/gtjluycxab.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tanke756.top/gtsskkveey.html

[E06] 替换子串
来源：http://hz.chenjidiqi.icu/gtpppimxbx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xinyue.icu/gtrqpmofty.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cashguo.top/gteycvoedl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.vqdsnc.cn/gtjxwwbaor.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtdwubvqjf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtsdydhbzu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guowangkeji.top/gtsdxzzwfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnqzz.top/gtybacrwwo.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gttzdqllkt.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtxvrambxd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sxryk.cn/gtxhvmyuik.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nwbrower.top/gtgbihilew.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.iojbl.cn/gtdvblqqlw.html

TS:   s.split(",")
来源：http://hz.tanke756.top/gtdsvhwgdh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hywenlv.cn/gtuieurguz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.c1oappe.top/gtxowaqqlp.html

Ruby: s.split(",");  s.split
来源：http://hz.redwolf501.top/gtdxfsuetm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.c1oappe.top/gtvjpgwmzd.html

[E08] 数组按分隔符合并
来源：http://hz.jlsjyb.cn/gtackjmdia.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gtzjdzvcyo.html

PHP:  implode(",", $items);
来源：http://hz.sysykeji.top/gtapqwxjkp.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtwzjejjhz.html

TS:   items.join(",")
来源：http://hz.yonumen.top/gtcmcijrwu.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtspaeyebm.html

Go:   strings.Join(items, ",")
来源：http://hz.chenzaomai.com/gtmjxixcnn.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtcnlnmzvc.html

C#:   string.Join(",", items)
来源：http://hz.jinyuanbaomall.cn/gtygrrraep.html

[E09] 去除所有空白字符
来源：http://hz.yj20258.top/gtycqtemkd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuanzx.com/gteafpytqn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gtmhlldctz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtcvbqbbhl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shangyingyoupin.top/gtxtpifzuh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhixingplan.top/gtgahajlwd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnxiangtu.top/gtuwsyuqld.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenjidiqi.icu/gtlkdmvufp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hysaishi.cn/gtcvwjeoei.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtnflujohv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtiheaxebj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yongpay.top/gtsovijtux.html

JS:   "7".padStart(3, "0")
来源：http://hz.9152youxi.cn/gtthsgjngr.html

TS:   "7".padStart(3, "0")
来源：http://hz.jiagoushi.top/gtybyqkfkd.html

Java: String.format("%03d", 7)
来源：http://hz.c1oappe.top/gtswmuvizj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtqggoclol.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xuanzx.com/gtocxnadpl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tianlin.xyz/gtunmnhlpl.html

[E11] 反转字符串
来源：http://hz.yj20258888.top/gtfduhmbld.html

Py:   s[::-1]
来源：http://hz.guowangkeji.top/gtjprcznki.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtaczojvun.html

JS:   [...s].reverse().join("")
来源：http://hz.xziqi.cn/gtioqayqss.html

TS:   [...s].reverse().join("")
来源：http://hz.hnqzz.top/gtjcgtunjh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hongshengwenyu.top/gtyuclpmuf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj202588.top/gttlrewxgg.html


<!-- 参考信息 -->