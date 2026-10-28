代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.yongpay.top/gtwbpkrpit.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnxiangtu.top/gtdpzikjgt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.wangdashe.top/gtkpnuscra.html

JS:   arr.slice(1, 4);
来源：http://hz.316326.xyz/gtcxvdjbqs.html

TS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtzxyaxcuf.html

Java: list.subList(1, 4);
来源：http://hz.52xcode.cn/gtlpumllos.html

Go:   arr[1:4]
来源：http://hz.nwbrower.top/gtarlxrzdj.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gtlvhdtply.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinghuilouyu.cn/gtlsfvwake.html

[D08] 合并两个数组
来源：http://hz.jiagoushi.top/gtcgdplukk.html

Py:   a + b;  a.extend(b)
来源：http://hz.yanxiufei.cn/gthfmmtsvn.html

PHP:  array_merge($a, $b);
来源：http://hz.pycfn.com/gtcfrlztjm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtgfegwmjw.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtqcnxxatb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.9152youxi.cn/gthnzucgiy.html

Go:   append(a, b...)
来源：http://hz.zhongyouzk.top/gtkecmcuvl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gthpexrqkk.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj202588.top/gtgnitjmsc.html

[D09] 排序（升序）
来源：http://hz.ydzc1.top/gtueoikpqa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.nanxuanxn.top/gtkpvtkmxh.html

PHP:  sort($arr);
来源：http://hz.yangfankeji.com/gtedxedobe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cucudq.cn/gtwdorsrbc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jiagoushi.top/gtmoqhgjgj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jianghu66.top/gtovuradjs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtqtlegmxv.html

Ruby: arr.sort
来源：http://hz.zhongyouzk.top/gtsfzlyglr.html

C#:   list.Sort();
来源：http://hz.birdmap.top/gtlclcyifz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ybcxt.top/gtuehfolbx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yvedp.cn/gtgoxrulnm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtowgntuok.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtxqfojtiv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtmlnqnneh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtuiwlsptt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hongshengwenyu.top/gtthbfxhxd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.haohaochexian.top/gtmmhtggjf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.52xcode.cn/gtphcihwws.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtootdfend.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.havefunace.top/gtxdzozirf.html

PHP:  array_reverse($arr);
来源：http://hz.xziqi.cn/gtnhsagurs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yangfankeji.com/gtsisvahhb.html

TS:   [...arr].reverse();
来源：http://hz.ydzc1.top/gtbjbaymlf.html

Java: Collections.reverse(list);
来源：http://hz.bjfxy.top/gtroubavgv.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtyrnzerds.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtwhnjkcuu.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtajtcoumf.html

[D12] 查找元素下标
来源：http://hz.xziqi.cn/gtarzsvhjn.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtzmqyqbpt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtedzupvfs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtfuxbthvf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gttwizghhs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.aibaodan.cn/gtdgcdklsd.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258888.top/gtmzirdnwd.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gtptjjibwj.html

C#:   list.IndexOf(x);
来源：http://hz.zycfv.cn/gtaokvnrvj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.smart0.xyz/gthlfxpfzk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.daxiang520.top/gtxkbiphpb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtslyitkgr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtgnqmcerq.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtcowrsmmg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ppjwa.cn/gtfunnntbd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhaomingkeji.xyz/gtczqicrvg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxuanxn.top/gtdqmnvifa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gzhubu.top/gtrqrptsdz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tanke756.top/gthcmeuwgw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ywan-chungtsiang.top/gthbronjer.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gtvpxyblyw.html

JS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gtansvwvcm.html

TS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtupsrrisl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.c1oappe.top/gtopdjcbqi.html

Go:   // 手写循环
来源：http://hz.dashuyun.cn/gtaafoubnr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtnydnnjnd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtslgvrspc.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtgakesbla.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gtgnjxjlzw.html

PHP:  array_unique($arr);
来源：http://hz.andypj.xyz/gtcozxaogy.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtgizmontj.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtkvwfzhto.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ehwqpu.com/gtgdiphulm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtonihwitn.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtmtregdxs.html

C#:   list.Distinct().ToList()
来源：http://hz.xuanzx.com/gtaiqljsnw.html

[D16] 求和与平均值
来源：http://hz.hysaishi.cn/gtnpvoqnpu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hysaishi.cn/gtukcmrnzv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gtrqwavzsg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gtysldzjnh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtccypnmtk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gzhubu.top/gtxxscxjkt.html

Go:   // 手写循环累加
来源：http://hz.zhijiandao.cn/gtrzzwoqfm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hnxiangtu.top/gtmenqefos.html

C#:   list.Sum();  list.Average()
来源：http://hz.cdnleiting.top/gtyfwtvcmi.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtvhncgpfv.html

Py:   max(arr);  min(arr)
来源：http://hz.ybcxt.top/gttfhowwux.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtuvkabbuw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gtppnyaehl.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gtyskeaplw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.aizwys.cn/gtltrantga.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtaqmtmpfw.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtelioqfqf.html

C#:   list.Max();  list.Min()
来源：http://hz.sysykeji.top/gtjcaamzro.html

[D18] 扁平化嵌套数组
来源：http://hz.dianchejie.cn/gtcrfhpozz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtavlpkbqc.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtvvqbnmkq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.iojbl.cn/gtzasdynrw.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtxoaxstey.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.smart0.xyz/gtlbjtsjqm.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtnhaichxv.html

Ruby: nested.flatten
来源：http://hz.sufxvd.cn/gtoxkjzreg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jyoumei.cn/gtqrabdciu.html

[D19] 按字段分组
来源：http://hz.aibaodan.cn/gtdkfkjwxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hongshengwenyu.top/gtuocyfttw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.gogol.net.cn/gtgtrlaglm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangshuangyany.cn/gtbxuqvbew.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gtmydpzyel.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yangfankeji.com/gtdvlkmhxc.html

Go:   // 手写 map[string][]T
来源：http://hz.52xcode.cn/gtigbzpwzl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhixingplan.top/gtcqhccltk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.wangdashe.top/gtujymygik.html

[D20] 统计每个元素出现次数
来源：http://hz.yanxiufei.cn/gtnowfqxnw.html

Py:   Counter(arr)
来源：http://hz.jqgufenzy.top/gtposbtwkf.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gteptrymrg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gtdcummrxi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtnkkotarj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.pengpengdd.cyou/gttfogjmza.html

Go:   // 手写 map[T]int
来源：http://hz.zhengqikj.top/gtxfolcqhz.html

Ruby: arr.tally
来源：http://hz.dashuyun.cn/gttwidvzqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtzlywjfau.html

[D21] 判断是否包含某元素
来源：http://hz.gaohongyu789.top/gtqjcwwwjx.html

Py:   x in arr
来源：http://hz.zdqjudy.top/gtyhognbhx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ppjwa.cn/gtunmljwhp.html

JS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtswultnqp.html

TS:   arr.includes(x)
来源：http://hz.svipenyu.cn/gthwuxxfgm.html

Java: list.contains(x)
来源：http://hz.vqdsnc.cn/gtitlgsqvw.html

Go:   slices.Contains(arr, x)
来源：http://hz.fengsongda.top/gtwsxegcvd.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtgjneglrr.html

C#:   list.Contains(x)
来源：http://hz.feifeiyinyue.top/gtrmqwstrx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.52xcode.cn/gtrqtykdkg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.haohaochexian.top/gtxgqpvtjc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gtnfnqwzzo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydjk.org.cn/gtdoaywrsp.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtejxkphmq.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtehnlavba.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtfrqdtvvr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shangyingyoupin.top/gtjnpdockd.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gteodvdpqe.html

[D23] reduce 累积计算
来源：http://hz.gzhubu.top/gtwyhohhpf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jianghu66.top/gtviirqfch.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gtzydedutf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtkfbuejrf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhengqikj.top/gtzcmjdwhf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.nwbrower.top/gtnuyqzujo.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtqoayzkpl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.dianchejie.cn/gtctorbsef.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gogol.net.cn/gtexgpivwe.html

[D24] 字典 / Map 基本操作
来源：http://hz.snrcjt.cn/gtsluwtkhv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.zhoulong.xyz/gtjbpqkisp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shangyingyoupin.top/gtkrghltjz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.dianchejie.cn/gtbzvursor.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jlsjyb.cn/gtpyfgmwgo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.iojbl.cn/gtnqistkpo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daxiang520.top/gthxncvbvh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.vqdsnc.cn/gtixdrvged.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinyuanbaomall.cn/gtafwpuiee.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtreeayrkk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yvedp.cn/gtchgskitg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydjk.org.cn/gtbtxoiwxt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ehwqpu.com/gtaejwuqgv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hammf.cn/gtatxwprpy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.tian-w.cn/gtvjzbmqet.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtkvkfcdqi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gaohongyu789.top/gtdpaekafk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.andypj.xyz/gtqrrekhmr.html

[D26] 数组转字符串
来源：http://hz.fengsongda.top/gtctibyjjy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shzxlz.cn/gtkrdglwsv.html

PHP:  implode(", ", $arr);
来源：http://hz.ehwqpu.com/gtkvwvawjc.html

JS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtodcpbnol.html

TS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtrmkaatcm.html

Java: String.join(", ", list)
来源：http://hz.daxiang520.top/gtpeglozom.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhengqikj.top/gtxrbajynk.html

Ruby: arr.join(", ")
来源：http://hz.sweek.top/gtqwdlklqh.html

C#:   string.Join(", ", list)
来源：http://hz.dashuyun.cn/gtavaioqww.html

================================================================================
来源：http://hz.jianghu66.top/gtspvdedbw.html

E. 字符串处理
来源：http://hz.meibo888.top/gtymlympub.html

================================================================================
来源：http://hz.xuanzx.com/gtkkhqeieb.html

[E01] 拼接字符串
来源：http://hz.yongpay.top/gtmhjwxtmr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jinqigfzy.top/gtequpvrhm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.kuanghao11.cn/gtjtpykhiy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zycfv.cn/gtrdgkfjkc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shuidangran.top/gtbmrvdbbf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jianghu66.top/gtswdoplpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtqjdruqys.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.c1oappe.top/gtmucqcoar.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtllhpzuvv.html

[E02] 重复字符串
来源：http://hz.9152youxi.cn/gtmvbhejpf.html

Py:   "ab" * 3
来源：http://hz.yj20258.top/gtygjqdtzc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinyuanbaomall.cn/gtfloikytm.html

JS:   "ab".repeat(3)
来源：http://hz.nanxuanxn.top/gtogrggycr.html

TS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtldwzblin.html

Java: "ab".repeat(3)
来源：http://hz.c1oappe.top/gtqukuxaal.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhiwuduotai.top/gtvdsudehs.html

Ruby: "ab" * 3
来源：http://hz.xinyue.icu/gtkavobfmf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cashguo.top/gtvqvivggv.html

[E03] 截取子串
来源：http://hz.yvedp.cn/gtwxoqptlk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yonumen.top/gtswxolazz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gzhubu.top/gtasfuqnjf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinghuilouyu.cn/gtrluybgsi.html

TS:   s.slice(1, 4)
来源：http://hz.yuanzhike.top/gtbjzpcqqa.html

Java: s.substring(1, 4)
来源：http://hz.ivvv.top/gtuwoizjsj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnqzz.top/gtcnsubzfj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.feifeiyinyue.top/gttfhzkyxx.html

C#:   s.Substring(1, 3)
来源：http://hz.dashuyun.cn/gthwkegdnz.html

[E04] 查找子串位置
来源：http://hz.316326.xyz/gtjdyrehma.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenzaomai.com/gtlhhozisq.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtzbcjfwak.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yueranfly.top/gtntwvewxa.html

TS:   s.indexOf("x")
来源：http://hz.aibaodan.cn/gtzduvyfbr.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gtotopkymi.html

Go:   strings.Index(s, "x")
来源：http://hz.hywenlv.cn/gttijjqiks.html

Ruby: s.index("x")
来源：http://hz.hywenlv.cn/gtkeceyqxo.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtcuhcavgk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yanxiufei.cn/gtkmbbogwv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hfpthk.cn/gtprtjggxr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtaxdamjua.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gthitaysmi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.wangdashe.top/gtsvgopzfj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtzdwpynar.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.bjfxy.top/gtlkivduas.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jyoumei.cn/gtdgnjnyiv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yonumen.top/gtbamutewd.html

[E06] 替换子串
来源：http://hz.redwolf501.top/gtdnyjarpn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhengqikj.top/gtwzbhbggy.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinghuilouyu.cn/gtbuiclxph.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gthkmzgpjr.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zdqjudy.top/gtmjyvlbnr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhongyouzk.top/gtywsnqwic.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtbuslasct.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shuidangran.top/gtmucmdzkd.html

C#:   s.Replace("a", "b")
来源：http://hz.xuanzx.com/gtqsshahgv.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtchnpfcnq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zdqjudy.top/gtjunkbstp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cdnleiting.top/gtvbtqenma.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xylfe.cn/gtdypsnyjr.html

TS:   s.split(",")
来源：http://hz.andypj.xyz/gtfqamrgqk.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.tanke756.top/gtnmkngwhp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtsswrnqoq.html

Ruby: s.split(",");  s.split
来源：http://hz.jinghuilouyu.cn/gtkerhowgo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.52xcode.cn/gtiscwbbeu.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtxmhnutul.html

Py:   ",".join(items)
来源：http://hz.fzhhl.top/gtqyxbnaqj.html

PHP:  implode(",", $items);
来源：http://hz.zycfv.cn/gtaiyavqla.html

JS:   items.join(",")
来源：http://hz.gogol.net.cn/gtykiukwgi.html

TS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtnwzrbtpy.html

Java: String.join(",", items)
来源：http://hz.zdqjudy.top/gtohlgkvan.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gtbedhacus.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtznloogbi.html

C#:   string.Join(",", items)
来源：http://hz.xingfuxueyuan.xyz/gtfxcehsqo.html

[E09] 去除所有空白字符
来源：http://hz.ydzc1.top/gtzfmccdgp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenzaomai.com/gtkqixdxih.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenzaomai.com/gtgncymkxk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.0kj1m.cn/gttezhxiku.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtmybdvdmx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zhoulong.xyz/gtjewrpges.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtivphhdhf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.snrcjt.cn/gtkcerctth.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.chenjidiqi.icu/gtpfponkgu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinyuanbaomall.cn/gtykvkhwzi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.gzhubu.top/gtbkzvtdao.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sweek.top/gtwelzszzh.html

JS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtztdfrwrq.html

TS:   "7".padStart(3, "0")
来源：http://hz.jqgufenzy.top/gtxntkthnq.html

Java: String.format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtydycmxap.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gtbfjiuvaf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.jyoumei.cn/gtxnhvqfoq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhengqikj.top/gtmlnlufzp.html

[E11] 反转字符串
来源：http://hz.zhixingplan.top/gtvehgzgqk.html

Py:   s[::-1]
来源：http://hz.yonumen.top/gtabvusrif.html

PHP:  strrev($s);
来源：http://hz.zhixingplan.top/gtmvzvykgz.html

JS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtttiwgypn.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtgpnpzevq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.snrcjt.cn/gtnrbxijwe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gtcpfdmlpf.html

Ruby: s.reverse
来源：http://hz.yj20258.top/gtdjfkcqxy.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigfzy.top/gtfgpwnlhx.html

[E12] 统计某字符出现次数
来源：http://hz.zhengqikj.top/gtknkcbxax.html

Py:   s.count("a")
来源：http://hz.shanyushiyangtech.top/gtcryltjed.html

PHP:  substr_count($s, "a");
来源：http://hz.cqqwz.cn/gtfbdoimyj.html

JS:   s.split("a").length - 1
来源：http://hz.xinyue.icu/gtwiwultpp.html

TS:   s.split("a").length - 1
来源：http://hz.jlsjyb.cn/gtswvoclex.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtclbadzbx.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gthbokhzei.html

Ruby: s.count("a")
来源：http://hz.bjfxy.top/gtcwnfbigc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgfzy.top/gtizrsydig.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtzzymyxui.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtdffwgeio.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gtmbxqstif.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gtwwmapqle.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pengpengdd.cyou/gtumejnjhh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cheryme.top/gtrhjcevyy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.316326.xyz/gtynhkrpsh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gtljbxisen.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gtwwckdfea.html


<!-- 参考信息 -->