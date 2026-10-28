代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.svipenyu.cn/gtgedmktsr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hnqzz.top/gtpvbwjkds.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ehwqpu.com/gtytygccfa.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtlwzkteqg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cheryme.top/gtxolafkau.html

[C15] 解构 / 展开参数
来源：http://hz.aibaodan.cn/gtqogqzeff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydzc1.top/gtashubrfs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.svipenyu.cn/gtuyncxnfk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhiwuduotai.top/gtrldgagqx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nwbrower.top/gtughskeks.html

Java: // 无解构
来源：http://hz.zycfv.cn/gtzusbpyxh.html

Go:   // 无解构
来源：http://hz.feifeiyinyue.top/gtmobmqifa.html

Ruby: a, b = pair
来源：http://hz.yj20258888.top/gtndtwgeii.html

C#:   var (a, b) = pair;
来源：http://hz.hnqzz.top/gtbfaxflir.html

[C16] 函数 / 方法重载
来源：http://hz.yuanzhike.top/gtjzgmyhvk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gtvedmigag.html

PHP:  // 无重载
来源：http://hz.shanyushiyangtech.top/gtrzxuiprx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.fzhhl.top/gtldqclrbv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.aibaodan.cn/gthpjjyaxe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zycfv.cn/gtfqumwzvj.html

Go:   // 无重载：用不同函数名
来源：http://hz.hywenlv.cn/gtzmzlmssm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pengpengdd.cyou/gtyeliyiem.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cqqwz.cn/gtpdsoeamr.html

================================================================================
来源：http://hz.hywenlv.cn/gtrsbqfizv.html

D. 数组 / 列表 / 集合
来源：http://hz.yj202588.top/gtndszogxc.html

================================================================================
来源：http://hz.9152youxi.cn/gtczcxddkr.html

[D01] 创建数组 / 列表
来源：http://hz.yueranfly.top/gtrnhwgtma.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtwernayuw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ydzc1.top/gtbrqziupn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hongshengwenyu.top/gtvssjzfqk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hammf.cn/gtlyrrqnmd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtbmxblymw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xinyue.icu/gtvygopvye.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tianlin.xyz/gtezxczagb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.nwbrower.top/gtucnmmydr.html

[D02] 追加元素到末尾
来源：http://hz.smart0.xyz/gtfkwhtnlo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sysykeji.top/gtecseqogu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fzhhl.top/gtuqkraigw.html

JS:   arr.push(4);
来源：http://hz.snrcjt.cn/gtlspudcmf.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtiqrlmhwf.html

Java: list.add(4);
来源：http://hz.ywan-chungtsiang.top/gtefsoghay.html

Go:   arr = append(arr, 4)
来源：http://hz.sysykeji.top/gtpqnbsahn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guannengcc.top/gtgihvayzs.html

C#:   list.Add(4);
来源：http://hz.yongpay.top/gtojwkrshw.html

[D03] 在指定位置插入元素
来源：http://hz.zdqjudy.top/gtlfszybno.html

Py:   arr.insert(0, 0)
来源：http://hz.haohaochexian.top/gtcbjaleib.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinqigufen.top/gtnyeenoxq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.feifeiyinyue.top/gthqowchjb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuxming.cn/gtsgatimuy.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtbqsnqwhj.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangdashe.top/gtpyqqbntv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hysaishi.cn/gtdawhhaww.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtpvydgtye.html

[D04] 删除元素
来源：http://hz.yvedp.cn/gtvykcjwmc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hnxiangtu.top/gtihnqzdwh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.svipenyu.cn/gthmczpmpa.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.wangdashe.top/gtuzifhxdn.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgufenzy.top/gtoemmuvan.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtsubdavzs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xinyue.icu/gthwyldwdf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yvedp.cn/gtmszizfdg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.meibo888.top/gtfububshx.html

[D05] 访问与修改元素
来源：http://hz.cdnleiting.top/gtrnyqqzqa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tian-w.cn/gtdswwmjtj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtkiowjmse.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtfsffbjad.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gotoacloud.top/gtslpvrzew.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigufen.top/gtqhhxlils.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gtlilphhgf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtittadibk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.316326.xyz/gtyqqdimiw.html

[D06] 数组长度
来源：http://hz.jlsjyb.cn/gtvzryozlf.html

Py:   len(arr)
来源：http://hz.zhiwuduotai.top/gtbwjuqmtf.html

PHP:  count($arr);
来源：http://hz.jlsjyb.cn/gtoschdhik.html

JS:   arr.length
来源：http://hz.yj20258.top/gttwxxcrow.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtthlfizwj.html

Java: list.size();
来源：http://hz.xziqi.cn/gtzsthbgkg.html

Go:   len(arr)
来源：http://hz.haohaochexian.top/gtakbxukgu.html

Ruby: arr.length; arr.size
来源：http://hz.xziqi.cn/gtqrjmuqym.html

C#:   list.Count;
来源：http://hz.daxiang520.top/gtgxhtrdyp.html

[D07] 切片 / 取子数组
来源：http://hz.yvedp.cn/gtozipultl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtylbgvlnv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnxiangtu.top/gtcirixgvh.html

JS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtipxgmaek.html

TS:   arr.slice(1, 4);
来源：http://hz.jinqigfzy.top/gtusovkmdj.html

Java: list.subList(1, 4);
来源：http://hz.jianghu66.top/gtkcrdjlbn.html

Go:   arr[1:4]
来源：http://hz.cheryme.top/gtrwhlbbhq.html

Ruby: arr[1, 3]
来源：http://hz.hywenlv.cn/gtmxwzgdpq.html

C#:   list.GetRange(1, 3);
来源：http://hz.cdnleiting.top/gtehvgurpc.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtxzokaudm.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtrvtoliru.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtzhybifut.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtkootngmv.html

TS:   [...a, ...b];
来源：http://hz.xylfe.cn/gtuxgtnolp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtaobapwoe.html

Go:   append(a, b...)
来源：http://hz.xuetiantiany.cn/gtasbvxpsg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj202588.top/gtflbnvlzz.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangshuangyany.cn/gtfqziyoka.html

[D09] 排序（升序）
来源：http://hz.daria6918.cn/gtstnyqzrr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtwpshvkzv.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtevyvjdby.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtazuymbqe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.316326.xyz/gtjfhoxyac.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtowzvjzbn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtslsmzdoe.html

Ruby: arr.sort
来源：http://hz.hywenlv.cn/gtakeqnqmh.html

C#:   list.Sort();
来源：http://hz.yuanzhike.top/gtxzwxsalx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.guowangkeji.top/gtijszeydn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gaohongyu789.top/gtezlnvcue.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.52xcode.cn/gtwmagubla.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtdzxbrbee.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigufen.top/gttoabvjxk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtxlzzfiha.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ywan-chungtsiang.top/gttuihotfe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtkwagtccw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yangfankeji.com/gtywiqoqmt.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtwrcyigth.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhijiandao.cn/gttgqmjtjk.html

PHP:  array_reverse($arr);
来源：http://hz.vqdsnc.cn/gtracbnrqr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtpqotwlnz.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtidvoubvk.html

Java: Collections.reverse(list);
来源：http://hz.yuanzhike.top/gtmookafqi.html

Go:   slices.Reverse(arr)
来源：http://hz.yangfankeji.com/gtrnevtgrs.html

Ruby: arr.reverse
来源：http://hz.yueranfly.top/gtdsqbqdxv.html

C#:   list.Reverse();
来源：http://hz.cdnleiting.top/gtdzjrneqf.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtpmxesmyv.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gthgsofehq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtagywziqn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydjk.org.cn/gtacoqbxhh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtaynbygak.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gtqvbrgpvr.html

Go:   slices.Index(arr, x)
来源：http://hz.quarkkingdee.top/gtqswecvnu.html

Ruby: arr.index(x)
来源：http://hz.shanyushiyangkeji.top/gtfzotjkch.html

C#:   list.IndexOf(x);
来源：http://hz.fengsongda.top/gtyqzkotey.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhaomingkeji.xyz/gtjelkupye.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gtqmdfknlq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ybcxt.top/gtkftipphr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtkludhrdn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yonumen.top/gtbkdxqnmv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dianchejie.cn/gtflqvuefj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtcpewpoub.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.fzhhl.top/gtgefnlunx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtvzqeivfr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.smart0.xyz/gtelafuxnz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xingfuxueyuan.xyz/gtnnlmreoe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cdnleiting.top/gtithvhakz.html

JS:   arr.map(x => x * 2)
来源：http://hz.yongpay.top/gthuwrhejj.html

TS:   arr.map(x => x * 2)
来源：http://hz.guowangkeji.top/gtzysgsbnh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xziqi.cn/gtjvonwwut.html

Go:   // 手写循环
来源：http://hz.zhaomingkeji.xyz/gtbznhljbz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtspntfqnb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenzaomai.com/gtoptoryyy.html

[D15] 去重
来源：http://hz.cashguo.top/gtzydunfef.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jianghu66.top/gtqzfqspso.html

PHP:  array_unique($arr);
来源：http://hz.jinghuilouyu.cn/gtvdbjnmxi.html

JS:   [...new Set(arr)]
来源：http://hz.zhaomingkeji.xyz/gtylzswmci.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtmfwlrknm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.birdmap.top/gtdburkana.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cqqwz.cn/gtmxgauftp.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtbtzgouhb.html

C#:   list.Distinct().ToList()
来源：http://hz.zhongyouzk.top/gtbzcajtdu.html

[D16] 求和与平均值
来源：http://hz.tanke756.top/gtdsrmzczg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.0kj1m.cn/gttsamhzrk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xuanzx.com/gthdlfbzul.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtkvcncsqz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtfafbkjsh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gtayksvmjn.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gtieregxpq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.haohaochexian.top/gtqoepgnku.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxinkj.top/gtpdmhrfcy.html

[D17] 最大值与最小值
来源：http://hz.jianghu66.top/gtwzhrpiyp.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtpjssbgit.html

PHP:  max($arr);  min($arr);
来源：http://hz.sufxvd.cn/gtkvtvmceh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jinqigufen.top/gtexdiutml.html

TS:   Math.max(...arr);
来源：http://hz.haohaochexian.top/gtalyowbul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sxryk.cn/gtilhptgdh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aizwys.cn/gtocvqrmcb.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtibdqzhaj.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtbecmbjzm.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gtitrumuzt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gtgmadrnne.html

PHP:  array_merge(...$nested);
来源：http://hz.gogol.net.cn/gtijfofaxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhaomingkeji.xyz/gticiyxouh.html

TS:   nested.flat();
来源：http://hz.yangfankeji.com/gtzapyovvb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daria6918.cn/gtpzzzpicz.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtiijndqsn.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gthjmylcan.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuanzhike.top/gtcgzysstz.html

[D19] 按字段分组
来源：http://hz.wangdashe.top/gtwkssmdch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.gzhubu.top/gtrxzbwpfw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hongshengwenyu.top/gtdxczclyf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtyphnlzkc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtgvrwryfg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.guowangkeji.top/gtcbxejrxc.html

Go:   // 手写 map[string][]T
来源：http://hz.gaohongyu789.top/gttsamihtr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinghuilouyu.cn/gtukrfwawr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jlsjyb.cn/gtwxxnlkpj.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtpfbygflv.html

Py:   Counter(arr)
来源：http://hz.jqgfzy.top/gtpxnhqkzi.html

PHP:  array_count_values($arr);
来源：http://hz.aizwys.cn/gtepzbuiqo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jyoumei.cn/gtnzdhkkor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenlongwang.top/gtfurtyzel.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jqgfzy.top/gtcskbonvj.html

Go:   // 手写 map[T]int
来源：http://hz.shuidangran.top/gtrvkjrwoi.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtivunjjsm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtugqfhnmw.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gtipqvmpkn.html

Py:   x in arr
来源：http://hz.jinqigufen.top/gtlvuhihwl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gogol.net.cn/gttxkjodsl.html

JS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtzbnyyyfh.html

TS:   arr.includes(x)
来源：http://hz.yonumen.top/gtdcbsaoxa.html

Java: list.contains(x)
来源：http://hz.sufxvd.cn/gtimywtdop.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj202588.top/gtlumwsaak.html

Ruby: arr.include?(x)
来源：http://hz.jlsjyb.cn/gtddfmocfe.html

C#:   list.Contains(x)
来源：http://hz.shzxlz.cn/gtkgxlevnb.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cheryme.top/gttcktzbjn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.c1oappe.top/gtqmofnvqs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xuetiantiany.cn/gtlxyebhoc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cqqwz.cn/gtucrcfrkh.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtygwsgigf.html

Java: new ArrayList<>(list);
来源：http://hz.cucudq.cn/gtyruvuvgg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.dashuyun.cn/gtgtalygte.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ppjwa.cn/gterxrevwe.html

C#:   new List<int>(list);
来源：http://hz.pycfn.com/gtejicysug.html

[D23] reduce 累积计算
来源：http://hz.0kj1m.cn/gttiainnlz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.feifeiyinyue.top/gtugicgcto.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fengsongda.top/gtzyfxvpad.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtqfyswvgy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtnshwbybv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gtodhkugen.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtflvjizwf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gtiogjbnkh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtqbjpyoro.html

[D24] 字典 / Map 基本操作
来源：http://hz.yongpay.top/gtggdffmtq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgufenzy.top/gtiyhixxme.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangdashe.top/gtczraitwc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shanyushiyangkeji.top/gttvryieks.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jianghu66.top/gtupagcqob.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtlhmlfljc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxuanxn.top/gtoaqdfrpo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hywenlv.cn/gtzgprikpq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhiwuduotai.top/gtbzrkazgl.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtokcjpevn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tanke756.top/gtuvsxzomg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.pengpengdd.cyou/gtuhccpjia.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.quarkkingdee.top/gtysywcxim.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.quarkkingdee.top/gtfpaivqxt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.jinqigfzy.top/gtgmrjyemd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.9152youxi.cn/gtklsehxek.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhijiandao.cn/gtuqlcdyyw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtqsklvfoh.html

[D26] 数组转字符串
来源：http://hz.cashguo.top/gtdszijakf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhixingplan.top/gtdeuivwwz.html

PHP:  implode(", ", $arr);
来源：http://hz.chenzaomai.com/gtgmnundpt.html

JS:   arr.join(", ")
来源：http://hz.jinqigfzy.top/gtuoulcazu.html

TS:   arr.join(", ")
来源：http://hz.dashuyun.cn/gtstqgombn.html

Java: String.join(", ", list)
来源：http://hz.aibaodan.cn/gtlvjuhrig.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtxxtrnhra.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gtwglkbctc.html

C#:   string.Join(", ", list)
来源：http://hz.ybcxt.top/gtwavxbpfv.html

================================================================================
来源：http://hz.xylfe.cn/gtmvsssgdb.html

E. 字符串处理
来源：http://hz.shangyingyoupin.top/gtmprmeiad.html

================================================================================
来源：http://hz.yj20258888.top/gtvvqchakc.html

[E01] 拼接字符串
来源：http://hz.zhoulong.xyz/gtugmjssvb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgufenzy.top/gthcrtkotr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cheryme.top/gtdzmphjmd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtgdaftjvx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cqqwz.cn/gtckznlkkr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtxytphxbv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aibaodan.cn/gtzcdhmmmr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.andypj.xyz/gtodysnzip.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.vqdsnc.cn/gtjtapswtg.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gteophjkff.html

Py:   "ab" * 3
来源：http://hz.chenlongwang.top/gtmwcjjmoi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hysaishi.cn/gtzqwzfgqa.html

JS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gtvtmzotns.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtusdydhii.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtqqylxrif.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xziqi.cn/gtlvxalewh.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtlzqggnic.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ehwqpu.com/gtqwonzehv.html

[E03] 截取子串
来源：http://hz.sweek.top/gtvaspxxfe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.smart0.xyz/gtqhzbedkq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jianghu66.top/gtialtzzlt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtgadwgbzn.html

TS:   s.slice(1, 4)
来源：http://hz.gzhubu.top/gtgjzkipfp.html

Java: s.substring(1, 4)
来源：http://hz.dashuyun.cn/gtxlfnvoig.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.sufxvd.cn/gtjubtmvci.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuanzx.com/gtkjlausss.html

C#:   s.Substring(1, 3)
来源：http://hz.yuanzhike.top/gtzgfftudu.html

[E04] 查找子串位置
来源：http://hz.yueranfly.top/gtyjbxmmma.html

Py:   s.find("x");  s.index("x")
来源：http://hz.nwbrower.top/gtqwkeaulg.html

PHP:  strpos($s, "x");
来源：http://hz.yanxiufei.cn/gtjiknvpdg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sxryk.cn/gtywjacpjb.html

TS:   s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtkuwvjdzz.html

Java: s.indexOf("x")
来源：http://hz.9152youxi.cn/gtocgbrxzz.html

Go:   strings.Index(s, "x")
来源：http://hz.fzhhl.top/gtgzgxjxpl.html

Ruby: s.index("x")
来源：http://hz.redwolf501.top/gtyqrvnlss.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtclxxkiyh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangdashe.top/gtdjhureyi.html


<!-- 参考信息 -->