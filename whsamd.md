代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yangfankeji.com/gtelsfapyu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sysykeji.top/gtlepygsle.html

[D05] 访问与修改元素
来源：http://hz.hywenlv.cn/gtsihkxgcu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gttapyypeo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangdashe.top/gthtgdtwir.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shuidangran.top/gtfnqgnvcv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.dianchejie.cn/gtsqeucmxd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jlsjyb.cn/gtwwzowgjh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtzklcvqub.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxinkj.top/gtjqutazhd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.52xcode.cn/gtgtxbrdjt.html

[D06] 数组长度
来源：http://hz.aibaodan.cn/gtjbagtnds.html

Py:   len(arr)
来源：http://hz.yangfankeji.com/gtadsrtteo.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtaavexeao.html

JS:   arr.length
来源：http://hz.yueranfly.top/gtquyxhoko.html

TS:   arr.length
来源：http://hz.0kj1m.cn/gtowgcyfcc.html

Java: list.size();
来源：http://hz.0kj1m.cn/gthrzfhcrv.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gthlgyhqtb.html

Ruby: arr.length; arr.size
来源：http://hz.meibo888.top/gtdjmilmdy.html

C#:   list.Count;
来源：http://hz.yj20258888.top/gtiluaizwp.html

[D07] 切片 / 取子数组
来源：http://hz.tianlin.xyz/gtjogunhxe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtlfnljgxh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuxming.cn/gtldubwlxk.html

JS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtypsmpqje.html

TS:   arr.slice(1, 4);
来源：http://hz.yueranfly.top/gtoregaxxt.html

Java: list.subList(1, 4);
来源：http://hz.yueranfly.top/gttgshjvfm.html

Go:   arr[1:4]
来源：http://hz.zhijiandao.cn/gtqzaajavw.html

Ruby: arr[1, 3]
来源：http://hz.jqgfzy.top/gtonemryqj.html

C#:   list.GetRange(1, 3);
来源：http://hz.sxryk.cn/gtkizyjqdr.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtuwismueh.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangtech.top/gtvccakdlj.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gtcqdgtumg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hysaishi.cn/gtijueuqwq.html

TS:   [...a, ...b];
来源：http://hz.mhx1999.top/gtvjmltrqh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtwikoihju.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtfughlpbh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.mhx1999.top/gtqahzbpjv.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnqzz.top/gtofqodrjt.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtvfabdpwd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtusgmaupb.html

PHP:  sort($arr);
来源：http://hz.xuanzx.com/gttetodwvy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sufxvd.cn/gtovehzvjq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hysaishi.cn/gtgizgxrae.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtykknagmg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.daria6918.cn/gtdkwmyuqe.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtftmzrxkx.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtkzizzepy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cqqwz.cn/gtwyjnghmo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtrqqrntzp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtgeergcuc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtkltfzxax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gtzxqahcda.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtopxcbmam.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aibaodan.cn/gtrrufxjmj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gtyotpltwu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xylfe.cn/gtdkolnukp.html

[D11] 反转数组
来源：http://hz.mhx1999.top/gtqdsbpkkq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gzhubu.top/gtbnhoofqk.html

PHP:  array_reverse($arr);
来源：http://hz.jianghu66.top/gtjryustnf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guowangkeji.top/gttwfosbgo.html

TS:   [...arr].reverse();
来源：http://hz.xuetiantiany.cn/gtsxmfrwqo.html

Java: Collections.reverse(list);
来源：http://hz.tanke756.top/gtiykfusnb.html

Go:   slices.Reverse(arr)
来源：http://hz.zhongyouzk.top/gtlpvsthbz.html

Ruby: arr.reverse
来源：http://hz.wangshuangyany.cn/gtrernaflo.html

C#:   list.Reverse();
来源：http://hz.birdmap.top/gtxpwwmghg.html

[D12] 查找元素下标
来源：http://hz.yj20258.top/gtprubjvoq.html

Py:   arr.index(x);  x in arr
来源：http://hz.haohaochexian.top/gthuvqwnru.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtwojyhceu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtacpzrcwx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtmdnezxdd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hammf.cn/gtivpvnqej.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxuanxn.top/gthrygxjhg.html

Ruby: arr.index(x)
来源：http://hz.hnqzz.top/gtsipqozfj.html

C#:   list.IndexOf(x);
来源：http://hz.jlsjyb.cn/gtlusxrdgj.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgfzy.top/gtedgbmzpv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgfzy.top/gtpybnlfkf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cheryme.top/gtjovyluyt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydjk.org.cn/gtgsqiraau.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxinkj.top/gtzzzyluvk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jiagoushi.top/gtjkkzqbqu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gtlvhqqsgd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.cdnleiting.top/gtgvxxpdxu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hysaishi.cn/gtojeamzoi.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aizwys.cn/gtojvhhntc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gthzbkfack.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.haohaochexian.top/gtcosjktqk.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gthdadqytq.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhijiandao.cn/gtopvfikxr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ppjwa.cn/gteowzqpbl.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtlglqnzwy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.kuanghao11.cn/gtfcinsvly.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yvedp.cn/gtjmlqxmoc.html

[D15] 去重
来源：http://hz.hongshengwenyu.top/gtukbbctwv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtwabltjhh.html

PHP:  array_unique($arr);
来源：http://hz.meibo888.top/gtzxrjtaia.html

JS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtrdohchoa.html

TS:   [...new Set(arr)]
来源：http://hz.shuidangran.top/gtjhegjuwd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gthqpaolkn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yj20258888.top/gtvtugcvrv.html

Ruby: arr.uniq
来源：http://hz.cashguo.top/gtkvzqyhlx.html

C#:   list.Distinct().ToList()
来源：http://hz.ydzc1.top/gttsldomxa.html

[D16] 求和与平均值
来源：http://hz.guowangkeji.top/gtwrjlpttm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.mhx1999.top/gtqmpjtjce.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtrlqqefwz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gzhubu.top/gtitglzxeh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gthxgqabcn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shanyushiyangkeji.top/gtuxjukwbu.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtknilnvag.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zycfv.cn/gtnochawaj.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtkyixmaeh.html

[D17] 最大值与最小值
来源：http://hz.dianchejie.cn/gtqpwcilhp.html

Py:   max(arr);  min(arr)
来源：http://hz.jinyuanbaomall.cn/gtvmupqhmr.html

PHP:  max($arr);  min($arr);
来源：http://hz.wangshuangyany.cn/gtpdldsumv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenjidiqi.icu/gttfgcsfzo.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gtezjfzfnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ivvv.top/gtoxmcnesu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtyzrlkouv.html

Ruby: arr.max;  arr.min
来源：http://hz.cqqwz.cn/gtxhaqtvds.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gtvdxcgmjh.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtfonqjxpz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.mhx1999.top/gtwmjhqebh.html

PHP:  array_merge(...$nested);
来源：http://hz.fzhhl.top/gtvfbapmwc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtxoghmvdf.html

TS:   nested.flat();
来源：http://hz.sysykeji.top/gtaezifgia.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yvedp.cn/gtjzxnlkas.html

Go:   // 手写双层循环
来源：http://hz.bjfxy.top/gtduqyqugr.html

Ruby: nested.flatten
来源：http://hz.yj202588.top/gthuncrgoe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hnqzz.top/gtcxgvqwmd.html

[D19] 按字段分组
来源：http://hz.zhixingplan.top/gtxwcbftxt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtdsyougsj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jianghu66.top/gtodhxsxbj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtxgxsoapf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cqqwz.cn/gtbftnclgz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gtkfmkhexo.html

Go:   // 手写 map[string][]T
来源：http://hz.0kj1m.cn/gtzvuobugq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hysaishi.cn/gtjulcuoai.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xinyue.icu/gtfdqjbftn.html

[D20] 统计每个元素出现次数
来源：http://hz.chenzaomai.com/gtwxjqykje.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gtjkdpjmyd.html

PHP:  array_count_values($arr);
来源：http://hz.hfpthk.cn/gtxpnnmzlr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtboksodzi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gtjnwosvve.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtovycxbkg.html

Go:   // 手写 map[T]int
来源：http://hz.shuidangran.top/gtacmplyha.html

Ruby: arr.tally
来源：http://hz.yj20258.top/gtqrklzmil.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pengpengdd.cyou/gtfyqdcggg.html

[D21] 判断是否包含某元素
来源：http://hz.xziqi.cn/gtypscfdrf.html

Py:   x in arr
来源：http://hz.hnxiangtu.top/gtzfwnanbs.html

PHP:  in_array($x, $arr, true);
来源：http://hz.meibo888.top/gtlmplwjsy.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtkiyocogv.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtntzorxai.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gthtfxoile.html

Go:   slices.Contains(arr, x)
来源：http://hz.guannengcc.top/gteoewjhar.html

Ruby: arr.include?(x)
来源：http://hz.hongshengwenyu.top/gtlrcxshce.html

C#:   list.Contains(x)
来源：http://hz.wangdashe.top/gtfqtsnden.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shanyushiyangkeji.top/gtmgoxsrra.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ywan-chungtsiang.top/gtsxanrrzd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xingfuxueyuan.xyz/gtwchsuluw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gtrjexygyx.html

TS:   [...arr];
来源：http://hz.sweek.top/gthfeowxov.html

Java: new ArrayList<>(list);
来源：http://hz.chenlongwang.top/gtbijrvbif.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuetiantiany.cn/gtrfzkoikq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hnxiangtu.top/gtmxumdwbx.html

C#:   new List<int>(list);
来源：http://hz.quarkkingdee.top/gtmwvygqhi.html

[D23] reduce 累积计算
来源：http://hz.jqgufenzy.top/gticjonrbv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhixingplan.top/gtdaodfmma.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zycfv.cn/gtkztgwmva.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtfvjpdrmp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtglplwtwu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtuotieble.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtcochriex.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtluuhkrxf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nwbrower.top/gtkmggiwdz.html

[D24] 字典 / Map 基本操作
来源：http://hz.dianchejie.cn/gthrqlqrhp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.birdmap.top/gtffdlbzhv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gthockkdtd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fengsongda.top/gtnqnufufk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.feifeiyinyue.top/gtiqzwqpgu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydzc1.top/gtylfoturo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtpwfzjkvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shuidangran.top/gtldzvqksz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangshuangyany.cn/gtohpqeakf.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtuuicrlrf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.meibo888.top/gtxjwgawja.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtvlswljbl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtosnwwbsj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dianchejie.cn/gtlpyblhcn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ybcxt.top/gtaevrnzrx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tian-w.cn/gtcfrslgnt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.daria6918.cn/gteokpsziv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gttpxaqlti.html

[D26] 数组转字符串
来源：http://hz.guowangkeji.top/gtwqsgkswr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.smart0.xyz/gtmihysejt.html

PHP:  implode(", ", $arr);
来源：http://hz.vqdsnc.cn/gtstlpokdb.html

JS:   arr.join(", ")
来源：http://hz.xingfuxueyuan.xyz/gtfwfvdgtv.html

TS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtmscfggzz.html

Java: String.join(", ", list)
来源：http://hz.0kj1m.cn/gtanmsoxoi.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhiwuduotai.top/gtiofnsbzz.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtgnkxltep.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtrrixiyjr.html

================================================================================
来源：http://hz.aizwys.cn/gtdliaeize.html

E. 字符串处理
来源：http://hz.yvedp.cn/gtedwercez.html

================================================================================
来源：http://hz.ehwqpu.com/gtgfylftym.html

[E01] 拼接字符串
来源：http://hz.pengpengdd.cyou/gtynbqfzrs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.quarkkingdee.top/gtsrkjzmzw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shzxlz.cn/gtzlgjpbuq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.9152youxi.cn/gthkzfexrm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ybcxt.top/gtdwycxyvv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.vqdsnc.cn/gthnofcpwk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zycfv.cn/gtbjewksdf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shuidangran.top/gtbvrufvpt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.havefunace.top/gtbsufdowj.html

[E02] 重复字符串
来源：http://hz.bjfxy.top/gtbfywdfta.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gtpewgeyye.html

PHP:  str_repeat("ab", 3);
来源：http://hz.9152youxi.cn/gtcyprvmdh.html

JS:   "ab".repeat(3)
来源：http://hz.zhiwuduotai.top/gtuyhfqlgj.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtbjihifoe.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtwhvgcxcs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtpnxmnxif.html

Ruby: "ab" * 3
来源：http://hz.wangdashe.top/gtetupsnyw.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhongyouzk.top/gttgiemvap.html

[E03] 截取子串
来源：http://hz.shuidangran.top/gtbfjnvdvx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtzyaosxfg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tianlin.xyz/gtvfxnakml.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtiehdzdru.html

TS:   s.slice(1, 4)
来源：http://hz.c1oappe.top/gtithtwqpm.html

Java: s.substring(1, 4)
来源：http://hz.jinqigufen.top/gteikxqsim.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.quarkkingdee.top/gttrbmhpay.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ehwqpu.com/gtlrrbiflc.html

C#:   s.Substring(1, 3)
来源：http://hz.yuxming.cn/gtdhdslyau.html

[E04] 查找子串位置
来源：http://hz.9152youxi.cn/gteqzmxkjt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.bjfxy.top/gtqpfucajr.html

PHP:  strpos($s, "x");
来源：http://hz.jqgfzy.top/gtdrlljnni.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yvedp.cn/gtevgskidf.html

TS:   s.indexOf("x")
来源：http://hz.yj202588.top/gtyeovtldc.html

Java: s.indexOf("x")
来源：http://hz.meibo888.top/gtbqiarnqo.html

Go:   strings.Index(s, "x")
来源：http://hz.bjfxy.top/gtatgohvnq.html

Ruby: s.index("x")
来源：http://hz.yangfankeji.com/gtrfnmtwlz.html

C#:   s.IndexOf("x")
来源：http://hz.sxryk.cn/gtumrizcif.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhaomingkeji.xyz/gtnbfoivbd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgfzy.top/gttjxgrosp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ybcxt.top/gtkbgzbwzs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangdashe.top/gtwdotvejs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gtpsyfuhsn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtuuqegntu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.haohaochexian.top/gtzzymcwqy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxinkj.top/gtsvdpsaxq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yongpay.top/gtxldqfrgm.html

[E06] 替换子串
来源：http://hz.zhongyouzk.top/gtbunnigyz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sufxvd.cn/gtciyqnkpe.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhongyouzk.top/gtstkklewq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtdamgbpzc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtagnxkwvu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenzaomai.com/gtkrgcbpms.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sufxvd.cn/gtdxselhdx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtqckhlgyi.html

C#:   s.Replace("a", "b")
来源：http://hz.havefunace.top/gtorlzesrh.html

[E07] 按分隔符拆分
来源：http://hz.jinyuanbaomall.cn/gttybseswv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ehwqpu.com/gtotftghju.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.andypj.xyz/gtgdbuekbl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gotoacloud.top/gtqwujuuxx.html

TS:   s.split(",")
来源：http://hz.cucudq.cn/gtpmzowlhd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.havefunace.top/gtrwwxsfev.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.smart0.xyz/gtwkzovbvs.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangkeji.top/gtjwrfllak.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yvedp.cn/gtvqonsxyv.html

[E08] 数组按分隔符合并
来源：http://hz.c1oappe.top/gtrsfadutp.html

Py:   ",".join(items)
来源：http://hz.chenlongwang.top/gtdxytygjl.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gtqswbeijh.html

JS:   items.join(",")
来源：http://hz.jinqigufen.top/gtjkixnors.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtrnlmdoul.html

Java: String.join(",", items)
来源：http://hz.redwolf501.top/gtzjkijfot.html

Go:   strings.Join(items, ",")
来源：http://hz.haohaochexian.top/gtmfqzdhqv.html

Ruby: items.join(",")
来源：http://hz.tianlin.xyz/gtvpvzbhqa.html

C#:   string.Join(",", items)
来源：http://hz.jyoumei.cn/gtgggvnydu.html

[E09] 去除所有空白字符
来源：http://hz.ivvv.top/gtbkrzvfyq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ybcxt.top/gtgmgmqmog.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shuidangran.top/gtlrieprhg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gaohongyu789.top/gtolfloqag.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtebxhzruw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xziqi.cn/gtlzzgwlnf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gtoqniqcix.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenzaomai.com/gtzjhhipwc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shuidangran.top/gteuflgcin.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenjidiqi.icu/gthpmwgwgf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shuidangran.top/gtkwedhfzy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.tianlin.xyz/gtjobzkjda.html

JS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtrzhlxbbq.html

TS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtjpigpizg.html

Java: String.format("%03d", 7)
来源：http://hz.tianlin.xyz/gteelugrex.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hfpthk.cn/gtjvwrkgtg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.bjfxy.top/gtciwlwray.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gaohongyu789.top/gtilaefayt.html

[E11] 反转字符串
来源：http://hz.redwolf501.top/gtdyzykkdh.html

Py:   s[::-1]
来源：http://hz.haohaochexian.top/gtcurvpvjc.html

PHP:  strrev($s);
来源：http://hz.hnxiangtu.top/gtdhkpqcrr.html

JS:   [...s].reverse().join("")
来源：http://hz.zhiwuduotai.top/gtovkhciuk.html

TS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtjtkdlgri.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.snrcjt.cn/gttyqixwen.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gthjshvftm.html


<!-- 参考信息 -->