代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtfcziuxjk.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtvydgxbdx.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yuanzhike.top/gtenuyyxnf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenzaomai.com/gtespfszse.html

C#:   list.Insert(0, 0);
来源：http://hz.xinyue.icu/gtvsrbijoi.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtnmccttut.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.smart0.xyz/gtjkhnvuqq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtowushfzf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gtzltjvydq.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtbrlcnoeh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangdashe.top/gtixhlvixg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nwbrower.top/gtdezuogqw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cdnleiting.top/gtxobgufpv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.aibaodan.cn/gtuvpqbfgr.html

[D05] 访问与修改元素
来源：http://hz.ydjk.org.cn/gtkzivjcjf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtonmeeubo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.tian-w.cn/gtymahzzor.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.iojbl.cn/gtrfmntitl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yongpay.top/gtdweexcav.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.aizwys.cn/gtkigqvsda.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zdqjudy.top/gtqxobtdoz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.dashuyun.cn/gtpbszofxw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guannengcc.top/gtrkagjvmi.html

[D06] 数组长度
来源：http://hz.9152youxi.cn/gtjmnietiq.html

Py:   len(arr)
来源：http://hz.chenjidiqi.icu/gttleplmgo.html

PHP:  count($arr);
来源：http://hz.andypj.xyz/gtrpkligpp.html

JS:   arr.length
来源：http://hz.cashguo.top/gtfokhxonh.html

TS:   arr.length
来源：http://hz.cucudq.cn/gtiloytajr.html

Java: list.size();
来源：http://hz.yuanzhike.top/gtssdbuqzd.html

Go:   len(arr)
来源：http://hz.yj202588.top/gtghfuabxr.html

Ruby: arr.length; arr.size
来源：http://hz.jiagoushi.top/gtqiecyziq.html

C#:   list.Count;
来源：http://hz.dianchejie.cn/gtmkujmspz.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtfyerruma.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.wangdashe.top/gtaudxfsqx.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jinghuilouyu.cn/gtbgfdfriu.html

JS:   arr.slice(1, 4);
来源：http://hz.bjfxy.top/gtdipnvexw.html

TS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gtaphuurgx.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtzydbhunr.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtelaetcbi.html

Ruby: arr[1, 3]
来源：http://hz.daria6918.cn/gtxjsffxsr.html

C#:   list.GetRange(1, 3);
来源：http://hz.yonumen.top/gtbgbnqevj.html

[D08] 合并两个数组
来源：http://hz.yj20258888.top/gtyvermcqy.html

Py:   a + b;  a.extend(b)
来源：http://hz.ydzc1.top/gtpwmqtqgr.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtkhyzlqcb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hammf.cn/gtwfeyuobl.html

TS:   [...a, ...b];
来源：http://hz.0kj1m.cn/gtlzuuplfh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.redwolf501.top/gtlyxtioul.html

Go:   append(a, b...)
来源：http://hz.gotoacloud.top/gtodgaahti.html

Ruby: a + b;  a.concat(b)
来源：http://hz.pengpengdd.cyou/gtyaxmnhsy.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnqzz.top/gtxgjiozkk.html

[D09] 排序（升序）
来源：http://hz.guannengcc.top/gtlbqqlypb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtgvdrwjlu.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gticvidbdb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtraeuvgbe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cucudq.cn/gthtokicub.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtdnibslzw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.0kj1m.cn/gtlixjtwbf.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtwsdhrfys.html

C#:   list.Sort();
来源：http://hz.sxryk.cn/gthvjbzfvx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jyoumei.cn/gtncaptjfq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xylfe.cn/gtochqiacm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenjidiqi.icu/gtkolxcqwk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtdshcligh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtaloapwhx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuanzhike.top/gtumvkvukr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gotoacloud.top/gtyndlyzyc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigfzy.top/gtrjdvzpoq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258888.top/gtsirwawpu.html

[D11] 反转数组
来源：http://hz.aibaodan.cn/gtthpchncj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj20258888.top/gtrdvbblfu.html

PHP:  array_reverse($arr);
来源：http://hz.zhixingplan.top/gtjzpavmhc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhoulong.xyz/gtcpzojoyb.html

TS:   [...arr].reverse();
来源：http://hz.jinghuilouyu.cn/gtimhfzivd.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtesmhgcdn.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigufen.top/gtiynibumb.html

Ruby: arr.reverse
来源：http://hz.xingfuxueyuan.xyz/gtunuyzszd.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gthskxybrv.html

[D12] 查找元素下标
来源：http://hz.yuxming.cn/gtnmdoegkd.html

Py:   arr.index(x);  x in arr
来源：http://hz.ppjwa.cn/gtlhwczyoz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.svipenyu.cn/gtbztzbvbf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtasbbukgu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtygyjclxq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhengqikj.top/gtaivfwwad.html

Go:   slices.Index(arr, x)
来源：http://hz.xuanzx.com/gtxmcgsjmv.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtmyzukajc.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtkuoekywh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gtzoyizkgy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gthbetuxwc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yonumen.top/gtfgklzttv.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gttcwxdurq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtfkldnfjz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yvedp.cn/gtbpxghwvn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nanxinkj.top/gttkpdnhxu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhoulong.xyz/gtrltdtgdu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gtyinlzymp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fzhhl.top/gtuntlgkbc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtfeluqikv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxinkj.top/gtfxbsxugx.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtmbanreaw.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtxqvhnnhh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangkeji.top/gtjmzrzkcq.html

Go:   // 手写循环
来源：http://hz.xylfe.cn/gtgkjvfivk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gogol.net.cn/gtccnpkjxz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daria6918.cn/gthvpalkzc.html

[D15] 去重
来源：http://hz.hysaishi.cn/gtlwgmvwju.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shangyingyoupin.top/gtdmulfmvq.html

PHP:  array_unique($arr);
来源：http://hz.ywan-chungtsiang.top/gtozwouody.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtswyknyum.html

TS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gturgzmdyq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ivvv.top/gtgmyqvkgs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ivvv.top/gtxnjkaoro.html

Ruby: arr.uniq
来源：http://hz.0kj1m.cn/gtqofkgekp.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtfmfcavbr.html

[D16] 求和与平均值
来源：http://hz.dashuyun.cn/gteovwtzci.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hongshengwenyu.top/gtglqinffo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yanxiufei.cn/gtvgtmtrlf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ehwqpu.com/gtxrtfpyyo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gthgzqoetz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtmpmocnak.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtfzusveqg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangshuangyany.cn/gtfliilrco.html

C#:   list.Sum();  list.Average()
来源：http://hz.gaohongyu789.top/gtmlbarqeu.html

[D17] 最大值与最小值
来源：http://hz.zhengqikj.top/gtewdlocxh.html

Py:   max(arr);  min(arr)
来源：http://hz.shanyushiyangkeji.top/gtltoudjdy.html

PHP:  max($arr);  min($arr);
来源：http://hz.ywan-chungtsiang.top/gthaqrthjx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtmwugdqjs.html

TS:   Math.max(...arr);
来源：http://hz.birdmap.top/gtdgdmnoaz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtofmlciqm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fzhhl.top/gtjisrwmkd.html

Ruby: arr.max;  arr.min
来源：http://hz.yongpay.top/gtvebkvygc.html

C#:   list.Max();  list.Min()
来源：http://hz.tanke756.top/gtvaxdevpq.html

[D18] 扁平化嵌套数组
来源：http://hz.jqgfzy.top/gtsoiusvel.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtcxqyrnte.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtxozuvned.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dianchejie.cn/gtpnhwmeft.html

TS:   nested.flat();
来源：http://hz.316326.xyz/gtrjqavnmu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yangfankeji.com/gtbmzkocko.html

Go:   // 手写双层循环
来源：http://hz.hnqzz.top/gtwqtqtlea.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtymzqpgxj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gzhubu.top/gtwjoeujso.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtsxtolroo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtyvpztiue.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guannengcc.top/gtxdzqooyh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtjdyqixca.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.9152youxi.cn/gtliwmnkai.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxinkj.top/gttyaywsbd.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtdfygbivy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ehwqpu.com/gtdwouspnh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtuvqwdwyt.html

[D20] 统计每个元素出现次数
来源：http://hz.sysykeji.top/gtphqyrsiv.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtcccukbwn.html

PHP:  array_count_values($arr);
来源：http://hz.dashuyun.cn/gtayxlxjid.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtqkdyldbf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtyudodtzb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.9152youxi.cn/gtisxbuclm.html

Go:   // 手写 map[T]int
来源：http://hz.hammf.cn/gtjiqtausv.html

Ruby: arr.tally
来源：http://hz.zhengqikj.top/gtahcmcbwe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hammf.cn/gtfribytzc.html

[D21] 判断是否包含某元素
来源：http://hz.yonumen.top/gtvskvgfoz.html

Py:   x in arr
来源：http://hz.hnqzz.top/gtcsuvkdef.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtkajckdop.html

JS:   arr.includes(x)
来源：http://hz.redwolf501.top/gtcbggesqn.html

TS:   arr.includes(x)
来源：http://hz.chenlongwang.top/gtqsgxycqd.html

Java: list.contains(x)
来源：http://hz.chenlongwang.top/gtbiepycqc.html

Go:   slices.Contains(arr, x)
来源：http://hz.iojbl.cn/gtusrlrqeg.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtlblwegbu.html

C#:   list.Contains(x)
来源：http://hz.xuetiantiany.cn/gtfpgkiewi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ehwqpu.com/gtesvszrrn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtwmarynil.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtgwnxpmcx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nwbrower.top/gtfkgxjdlp.html

TS:   [...arr];
来源：http://hz.dashuyun.cn/gtwuagqyhb.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtpqynliiv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.andypj.xyz/gtjxxqdgbd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtryupwetm.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtoqcaralv.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gtvdnrqnnn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtehmjigcz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxuanxn.top/gthhtmjejg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtbwpeoesi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gthvsambiv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.316326.xyz/gtjfnplqlz.html

Go:   // 手写循环
来源：http://hz.smart0.xyz/gthdyaugeb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenzaomai.com/gtjobuaiey.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sufxvd.cn/gtzhfqzycx.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtbaizsqug.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtlpjksues.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.0kj1m.cn/gtxlkhvxsy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.kuanghao11.cn/gtmmuvxiho.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.haohaochexian.top/gtxxwjyizm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtrjyfxnlf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhongyouzk.top/gtyhfnoosc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sysykeji.top/gtkuraqqsm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtcqofmlbv.html

[D25] Set 集合去重与交并差
来源：http://hz.316326.xyz/gtpthrrkqs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.havefunace.top/gteyoqafij.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yangfankeji.com/gtgpevcnka.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.52xcode.cn/gtghstyztc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gotoacloud.top/gtctnplakd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yonumen.top/gtgxbntmxw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jiagoushi.top/gtfgochvga.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yongpay.top/gtlrsuaejg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.daxiang520.top/gtogwahxbb.html

[D26] 数组转字符串
来源：http://hz.cashguo.top/gtjdyvuhcr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jqgufenzy.top/gtoarelbye.html

PHP:  implode(", ", $arr);
来源：http://hz.shanyushiyangkeji.top/gtzhssvaor.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtyhfegchr.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtzfbatfvs.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtltffwrmf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cheryme.top/gtveapizou.html

Ruby: arr.join(", ")
来源：http://hz.hnxiangtu.top/gtwcumfiaq.html

C#:   string.Join(", ", list)
来源：http://hz.cdnleiting.top/gtieczhyps.html

================================================================================
来源：http://hz.ivvv.top/gtiemzteat.html

E. 字符串处理
来源：http://hz.yuxming.cn/gtcbulbepu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtidrtlfeb.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtohhlfqkm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sweek.top/gtgajphdab.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xinyue.icu/gtlighohdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenlongwang.top/gtvddutwjq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daxiang520.top/gtdqqxobmc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gtgkwbfxzj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj20258888.top/gtdrwupldy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtitkhoutf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gtkehwrpce.html

[E02] 重复字符串
来源：http://hz.nanxinkj.top/gtlurgzvbv.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtdmhgjqoq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xingfuxueyuan.xyz/gtcoiepozo.html

JS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtbxajruvp.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gteojomapg.html

Java: "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtyrlxcpvy.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gtezqkbzut.html

Ruby: "ab" * 3
来源：http://hz.hfpthk.cn/gtiyxlgbao.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtugictaaa.html

[E03] 截取子串
来源：http://hz.yongpay.top/gtqvmuksrn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jianghu66.top/gtrljrmufq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.chenzaomai.com/gtqdqbrbxp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtkxczlmwx.html

TS:   s.slice(1, 4)
来源：http://hz.cucudq.cn/gtalleenkd.html

Java: s.substring(1, 4)
来源：http://hz.ywan-chungtsiang.top/gtkfzkddup.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtstvmytso.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.52xcode.cn/gtjjauvrtw.html

C#:   s.Substring(1, 3)
来源：http://hz.nwbrower.top/gtkghbioll.html

[E04] 查找子串位置
来源：http://hz.pengpengdd.cyou/gtipvwpbjp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtxeikpcmj.html

PHP:  strpos($s, "x");
来源：http://hz.jianghu66.top/gtgykoghpw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pycfn.com/gtruaxdgpi.html

TS:   s.indexOf("x")
来源：http://hz.xinyue.icu/gtonmdyepi.html

Java: s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtnpfqcyfz.html

Go:   strings.Index(s, "x")
来源：http://hz.zhiwuduotai.top/gtrfmkuyta.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtbjixqwyn.html

C#:   s.IndexOf("x")
来源：http://hz.hnqzz.top/gtdvkepnfs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhoulong.xyz/gtismbjxom.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xingfuxueyuan.xyz/gtsyeuolfk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gttqhmwsvx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtcldbkrkq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtbwupnbvk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fzhhl.top/gtmivzcntz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.haohaochexian.top/gtaypulvqn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtfneknlsm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xziqi.cn/gtqzupcofc.html

[E06] 替换子串
来源：http://hz.xziqi.cn/gtovdufokg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gthhqafcve.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.52xcode.cn/gtlngtaktl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtemqmmrks.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtdorakngy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.9152youxi.cn/gtckiliwhn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.gzhubu.top/gtdflakrxm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhongyouzk.top/gtwhfobrpg.html

C#:   s.Replace("a", "b")
来源：http://hz.wangdashe.top/gtlnmmbavu.html

[E07] 按分隔符拆分
来源：http://hz.yvedp.cn/gticvlcflt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hywenlv.cn/gtffnqzsvv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.wangdashe.top/gtojtrpaie.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xziqi.cn/gtsjuibskh.html

TS:   s.split(",")
来源：http://hz.daria6918.cn/gtphhewhdh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.dianchejie.cn/gtuxsbwttj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.wangdashe.top/gtwlbwdgif.html

Ruby: s.split(",");  s.split
来源：http://hz.aizwys.cn/gtiogbcgwl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yueranfly.top/gtnetbunio.html

[E08] 数组按分隔符合并
来源：http://hz.sysykeji.top/gtxnkbvexi.html

Py:   ",".join(items)
来源：http://hz.dashuyun.cn/gtdbriwxqg.html

PHP:  implode(",", $items);
来源：http://hz.tian-w.cn/gtqxtnvklq.html

JS:   items.join(",")
来源：http://hz.tianlin.xyz/gtnzbwajob.html

TS:   items.join(",")
来源：http://hz.shuidangran.top/gttzrneask.html

Java: String.join(",", items)
来源：http://hz.hongshengwenyu.top/gtcscdccbl.html

Go:   strings.Join(items, ",")
来源：http://hz.shzxlz.cn/gthkbzxjdw.html

Ruby: items.join(",")
来源：http://hz.meibo888.top/gtsazmybxe.html

C#:   string.Join(",", items)
来源：http://hz.jinghuilouyu.cn/gttsespccf.html

[E09] 去除所有空白字符
来源：http://hz.feifeiyinyue.top/gtjhcbjkax.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dashuyun.cn/gtbjnqhvfk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtbqcypqrl.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtfzeqvnmh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.svipenyu.cn/gtdjeymuuf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cqqwz.cn/gtoxrhdhfl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtrxxiexbd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hammf.cn/gtdwvxkyuf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hfpthk.cn/gtgaqjqyqg.html

[E10] 左侧补零 / 定长填充
来源：http://hz.guannengcc.top/gtyefjaqrn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gaohongyu789.top/gtkllfttvz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtfkrvkzro.html

JS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtdcazqbqp.html


<!-- 参考信息 -->