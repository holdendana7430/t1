代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gteaxeywij.html

[C15] 解构 / 展开参数
来源：http://hz.xingfuxueyuan.xyz/gtxvsyilaj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258.top/gtpejcrtlx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ybcxt.top/gtcjkehigf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zhiwuduotai.top/gtuhdzzqww.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhaomingkeji.xyz/gtfncwxznz.html

Java: // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtcbasplbs.html

Go:   // 无解构
来源：http://hz.hywenlv.cn/gtdbjpvurd.html

Ruby: a, b = pair
来源：http://hz.zdqjudy.top/gtyvuyhdld.html

C#:   var (a, b) = pair;
来源：http://hz.sxryk.cn/gttxicbkvl.html

[C16] 函数 / 方法重载
来源：http://hz.gzhubu.top/gthgqtnbqb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yanxiufei.cn/gtvjxqxyta.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtqwbcpghd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.guowangkeji.top/gteecpabwm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.iojbl.cn/gtuhvaynsy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hnqzz.top/gtlhussqcl.html

Go:   // 无重载：用不同函数名
来源：http://hz.52xcode.cn/gtujojxpnd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gaohongyu789.top/gtzggrrxkk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pycfn.com/gtnrffqvrs.html

================================================================================
来源：http://hz.gzhubu.top/gtnhpavzyd.html

D. 数组 / 列表 / 集合
来源：http://hz.52xcode.cn/gtrepsxbrd.html

================================================================================
来源：http://hz.quarkkingdee.top/gtxdtrcind.html

[D01] 创建数组 / 列表
来源：http://hz.vqdsnc.cn/gtjcarztir.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhoulong.xyz/gtgdtcirrs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xylfe.cn/gtyawkfupt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xinyue.icu/gtfwmbzdpv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtehddwhfu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ybcxt.top/gtqscaqlbr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtlvpvnuup.html

Ruby: arr = [1, 2, 3]
来源：http://hz.daxiang520.top/gtvnjpoghw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pengpengdd.cyou/gtmqawtump.html

[D02] 追加元素到末尾
来源：http://hz.ydjk.org.cn/gtqucrykbs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.cheryme.top/gtrbjrwhly.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.ivvv.top/gtzlpewwnx.html

JS:   arr.push(4);
来源：http://hz.sxryk.cn/gtmsclfcyj.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangtech.top/gtdlxgbvop.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtitwxlmxt.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gtypdfmuck.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.cqqwz.cn/gtzluijmgr.html

C#:   list.Add(4);
来源：http://hz.hongshengwenyu.top/gtxbtodbkz.html

[D03] 在指定位置插入元素
来源：http://hz.pengpengdd.cyou/gtynfgmuna.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangkeji.top/gtbexicgxo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhengqikj.top/gtlygsjmnw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenjidiqi.icu/gtwamklbqu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ywan-chungtsiang.top/gthdfhafiq.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtsxshqxsr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gaohongyu789.top/gtgbvkbytw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnqzz.top/gtqyhukdaa.html

C#:   list.Insert(0, 0);
来源：http://hz.chenlongwang.top/gtpfaoygbu.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtzzwlhouh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shangyingyoupin.top/gtbptdzcqt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.9152youxi.cn/gtlmtrpfdx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shangyingyoupin.top/gthsrbbyef.html

TS:   arr.splice(0, 1);
来源：http://hz.yueranfly.top/gtlnkyfypk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.aibaodan.cn/gtejxifsmp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnxiangtu.top/gteoxwojjl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hysaishi.cn/gtlcilhqmh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yvedp.cn/gteqjtqncl.html

[D05] 访问与修改元素
来源：http://hz.jinyuanbaomall.cn/gtllxifbwo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtfntchmjs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtfzqjmjif.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hnqzz.top/gtwobqyxtl.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhoulong.xyz/gtnkdwdeyt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gtdjlpkskv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtvofuhvvr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtkvgphwvi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.cashguo.top/gtqoegadfa.html

[D06] 数组长度
来源：http://hz.yanxiufei.cn/gtvojnayzh.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gtelyrcjzo.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtqozoywfs.html

JS:   arr.length
来源：http://hz.gzhubu.top/gtohmmspwl.html

TS:   arr.length
来源：http://hz.hongshengwenyu.top/gtxbbbrwiv.html

Java: list.size();
来源：http://hz.hongshengwenyu.top/gthsrkuoso.html

Go:   len(arr)
来源：http://hz.zhijiandao.cn/gtkiriclno.html

Ruby: arr.length; arr.size
来源：http://hz.quarkkingdee.top/gtyrnigrti.html

C#:   list.Count;
来源：http://hz.gzhubu.top/gtpkidkmtc.html

[D07] 切片 / 取子数组
来源：http://hz.ivvv.top/gtbdodxvie.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtamxoirtt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnqzz.top/gtrhjpzpuf.html

JS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtabnfxgrv.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtmhxohdnm.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtopmbvbpk.html

Go:   arr[1:4]
来源：http://hz.jqgfzy.top/gtjsfvhkqq.html

Ruby: arr[1, 3]
来源：http://hz.xinyue.icu/gtylohgurt.html

C#:   list.GetRange(1, 3);
来源：http://hz.andypj.xyz/gtgcthtdxy.html

[D08] 合并两个数组
来源：http://hz.jinyuanbaomall.cn/gtzyvxwfir.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtwqxjktpm.html

PHP:  array_merge($a, $b);
来源：http://hz.guowangkeji.top/gtimfuyfqa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xziqi.cn/gtmqxuevup.html

TS:   [...a, ...b];
来源：http://hz.zhaomingkeji.xyz/gtwjlglfks.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgfzy.top/gtlrtaezcl.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtvsmnmecr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gzhubu.top/gtndrxmvmm.html

C#:   a.Concat(b).ToList()
来源：http://hz.hongshengwenyu.top/gtnjnmjncu.html

[D09] 排序（升序）
来源：http://hz.hongshengwenyu.top/gtqpiycgih.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtlxwotzhy.html

PHP:  sort($arr);
来源：http://hz.gaohongyu789.top/gtgeeklcbu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.haohaochexian.top/gtczlroqkj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gtltugfqmh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hnqzz.top/gteakocofv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hfpthk.cn/gtxzfcimwc.html

Ruby: arr.sort
来源：http://hz.ydzc1.top/gtwdaptbxw.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gttjwvwhvd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.chenzaomai.com/gtektdunav.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gtdopgouep.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtohflipah.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtivmvlgsz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtaqholffx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ywan-chungtsiang.top/gtzpbktqcl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cucudq.cn/gtjyvhdook.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hfpthk.cn/gthsngrhbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xinyue.icu/gtybbseqvr.html

[D11] 反转数组
来源：http://hz.xuetiantiany.cn/gttmhyrpvy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gtcmogyfhd.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangkeji.top/gtxsqshmvu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.vqdsnc.cn/gtpraapzil.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtwhwaaucd.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gtfoijcbfq.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gthphdwujc.html

Ruby: arr.reverse
来源：http://hz.kuanghao11.cn/gtxvdzznhb.html

C#:   list.Reverse();
来源：http://hz.cashguo.top/gtmbrmbrwj.html

[D12] 查找元素下标
来源：http://hz.cdnleiting.top/gtzqdggjep.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydzc1.top/gtfvlxnhpy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shangyingyoupin.top/gtuppwokgu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.vqdsnc.cn/gtmrkhptjc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhixingplan.top/gtpinqxnrk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xylfe.cn/gtjgqtyiee.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtzyqjthzz.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtmsfkksow.html

C#:   list.IndexOf(x);
来源：http://hz.jinghuilouyu.cn/gtaqqwuuft.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ywan-chungtsiang.top/gtpejfdulp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yangfankeji.com/gtdfpwkhsy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gthceomtfz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtpzcqvosm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dashuyun.cn/gtgssrkthd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yanxiufei.cn/gtheeautkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtwjxwgmdr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigfzy.top/gtozkiqihz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.xylfe.cn/gtbprtipvs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigfzy.top/gtvcabzuho.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gtxtgagjwc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.quarkkingdee.top/gtzzvynzue.html

JS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtmdddnspp.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtsbtgazku.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtizjrskrj.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtuffbzhky.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gtppnwdzwf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.birdmap.top/gtmsldlfhz.html

[D15] 去重
来源：http://hz.ydjk.org.cn/gtdqkylycl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtkalnhpqv.html

PHP:  array_unique($arr);
来源：http://hz.gotoacloud.top/gtdnrxwhir.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtiycdrpsr.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtmfaonagw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtwjligjwb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shzxlz.cn/gtsfemwcrp.html

Ruby: arr.uniq
来源：http://hz.ywan-chungtsiang.top/gtcdwuhnsz.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigufen.top/gtfxhppekk.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtlzxznfmq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gtjdzqrasx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gttklfrdkh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sweek.top/gtzlzgypif.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtsdiccmzy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.shangyingyoupin.top/gtjjlukcpv.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gthtzllfok.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtybbgwoiv.html

C#:   list.Sum();  list.Average()
来源：http://hz.ydjk.org.cn/gtwwqnnuhb.html

[D17] 最大值与最小值
来源：http://hz.pengpengdd.cyou/gtfeymijai.html

Py:   max(arr);  min(arr)
来源：http://hz.gzhubu.top/gtfdilcxec.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtidkxidna.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtbyqojhvw.html

TS:   Math.max(...arr);
来源：http://hz.zhongyouzk.top/gtiieledjh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.birdmap.top/gtvdpvbomb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtdfgznpqt.html

Ruby: arr.max;  arr.min
来源：http://hz.zhixingplan.top/gtyurgnxpl.html

C#:   list.Max();  list.Min()
来源：http://hz.iojbl.cn/gteygfjnpr.html

[D18] 扁平化嵌套数组
来源：http://hz.sweek.top/gtmaplinqe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuanzhike.top/gtnzxtvsba.html

PHP:  array_merge(...$nested);
来源：http://hz.jinyuanbaomall.cn/gtwzpvxtfw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shuidangran.top/gtswmvgqbu.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtzthjbmkm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.chenlongwang.top/gthgqkmyfu.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtauixlqxp.html

Ruby: nested.flatten
来源：http://hz.zycfv.cn/gtrbvjmjbz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtmljsudpz.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtesjmxint.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gthvfthgpc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.kuanghao11.cn/gtpsacnywz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinghuilouyu.cn/gtvvpqsaty.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shuidangran.top/gtnhdgcwwx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gttnxqxfwh.html

Go:   // 手写 map[string][]T
来源：http://hz.nwbrower.top/gtsenbquqq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guowangkeji.top/gtslladjdj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.andypj.xyz/gtegvcfrvt.html

[D20] 统计每个元素出现次数
来源：http://hz.yongpay.top/gtllidzdmc.html

Py:   Counter(arr)
来源：http://hz.yuanzhike.top/gthbhwnjzf.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtcirseofg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtoylcqvhf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtdzwmpndb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtxywiwmou.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gtqfybbljn.html

Ruby: arr.tally
来源：http://hz.jlsjyb.cn/gtoqsocrxj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinyuanbaomall.cn/gtqaftbhrx.html

[D21] 判断是否包含某元素
来源：http://hz.52xcode.cn/gtxxbsugqk.html

Py:   x in arr
来源：http://hz.pycfn.com/gtnqzwctnq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.haohaochexian.top/gtxxokrkqr.html

JS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtwvagjtil.html

TS:   arr.includes(x)
来源：http://hz.tanke756.top/gtunkrejav.html

Java: list.contains(x)
来源：http://hz.zycfv.cn/gtfvjsbups.html

Go:   slices.Contains(arr, x)
来源：http://hz.snrcjt.cn/gtdgesnfni.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtthmhefmi.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gtdefufhnk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.fengsongda.top/gtjrwtendp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtxrxxmzqz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hammf.cn/gtjlwoyvfk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.quarkkingdee.top/gtrmtgacek.html

TS:   [...arr];
来源：http://hz.kuanghao11.cn/gtjjtakxou.html

Java: new ArrayList<>(list);
来源：http://hz.cheryme.top/gtjhhowehm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ivvv.top/gtpbaxdasf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtjxlnaykm.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtibpmnuft.html

[D23] reduce 累积计算
来源：http://hz.cucudq.cn/gtwqugkdui.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinyuanbaomall.cn/gtjmrnjsne.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtcqloxpqs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtcvvqjoxu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtihabgygm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.guowangkeji.top/gtyuswdrbr.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gteqezypky.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.kuanghao11.cn/gtoxwcqpaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tanke756.top/gtjgzytdvf.html

[D24] 字典 / Map 基本操作
来源：http://hz.c1oappe.top/gtlkesaqet.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtpwkfuejb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.snrcjt.cn/gtnwgvdvcf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hammf.cn/gtmkxvijny.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xinyue.icu/gtrgmlrufq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhaomingkeji.xyz/gtqjezppwx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtgjnszeib.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cashguo.top/gtjwnwyrqs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangdashe.top/gtokhzntku.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtihuyceux.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ywan-chungtsiang.top/gtbcvysbaf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yueranfly.top/gtwwfdopgg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hywenlv.cn/gtywifvdha.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yangfankeji.com/gtddvtmfgt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gttihnjigb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtndxfkfyk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangtech.top/gtcnmmjgkc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shuidangran.top/gtysegorqw.html

[D26] 数组转字符串
来源：http://hz.xziqi.cn/gtprpoahgo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtghvgrptr.html

PHP:  implode(", ", $arr);
来源：http://hz.hywenlv.cn/gtgwfezwdd.html

JS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtbecokifu.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtxfddtefd.html

Java: String.join(", ", list)
来源：http://hz.chenlongwang.top/gtytdemczu.html

Go:   strings.Join(strs, ", ")
来源：http://hz.c1oappe.top/gtaevjptzb.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gtangucbot.html

C#:   string.Join(", ", list)
来源：http://hz.cheryme.top/gtnwkqkvaf.html

================================================================================
来源：http://hz.sysykeji.top/gtgftgtegt.html

E. 字符串处理
来源：http://hz.aibaodan.cn/gtmyetlbrh.html

================================================================================
来源：http://hz.ybcxt.top/gtxogxorko.html

[E01] 拼接字符串
来源：http://hz.snrcjt.cn/gtlcrhbnxp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gtnaztscql.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.9152youxi.cn/gtzyoktpda.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtktjsngyu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gttocmumvf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.0kj1m.cn/gtvryqlwpg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.ehwqpu.com/gtyivhaked.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinqigfzy.top/gthpqhpcjq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigufen.top/gtshcgrgjs.html

[E02] 重复字符串
来源：http://hz.yj202588.top/gtvtalepdj.html

Py:   "ab" * 3
来源：http://hz.xuetiantiany.cn/gtwcprehlh.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtrghqvbhx.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtkodtzrke.html

TS:   "ab".repeat(3)
来源：http://hz.quarkkingdee.top/gtetrutlfl.html

Java: "ab".repeat(3)
来源：http://hz.fzhhl.top/gtitltibcw.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gaohongyu789.top/gtfgnkrbba.html

Ruby: "ab" * 3
来源：http://hz.cheryme.top/gtapimddda.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.tianlin.xyz/gttvsjoasz.html

[E03] 截取子串
来源：http://hz.jinyuanbaomall.cn/gttdaffikk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.birdmap.top/gtxvwdedaj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.nanxinkj.top/gtshrueavt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.0kj1m.cn/gtjhiyfpbi.html

TS:   s.slice(1, 4)
来源：http://hz.hywenlv.cn/gtkduocabz.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtgnhhtkmj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.shuidangran.top/gtctkfmuhu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shzxlz.cn/gtzwkkcyea.html

C#:   s.Substring(1, 3)
来源：http://hz.pengpengdd.cyou/gtqjxuxhjh.html

[E04] 查找子串位置
来源：http://hz.snrcjt.cn/gtnejxtrqr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.havefunace.top/gtblrvihcw.html

PHP:  strpos($s, "x");
来源：http://hz.pengpengdd.cyou/gtsexsknko.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj20258.top/gtvdoqntgr.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtsebbpufe.html

Java: s.indexOf("x")
来源：http://hz.ppjwa.cn/gtzcnkcysh.html

Go:   strings.Index(s, "x")
来源：http://hz.feifeiyinyue.top/gtkoycrrqw.html

Ruby: s.index("x")
来源：http://hz.nanxinkj.top/gtxfyqzgjs.html

C#:   s.IndexOf("x")
来源：http://hz.c1oappe.top/gtsmdmbfow.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yonumen.top/gtiytamdmi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.birdmap.top/gtjrohofns.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jlsjyb.cn/gtoetmhuqn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.c1oappe.top/gtinvryndb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhoulong.xyz/gteqrxkgke.html


<!-- 参考信息 -->