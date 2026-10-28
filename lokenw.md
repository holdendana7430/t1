代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.0kj1m.cn/gtbaszukhm.html

Go:   func add(a, b int) int
来源：http://hz.kuanghao11.cn/gthazfchlo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ydjk.org.cn/gtknxxwhqu.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenjidiqi.icu/gtabfsdkmp.html

[C14] 泛型函数
来源：http://hz.vqdsnc.cn/gtxzlgenmc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuetiantiany.cn/gtifxoyfoz.html

PHP:  // 无泛型
来源：http://hz.c1oappe.top/gtwwxsdpkf.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtsmawfmqy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gteinibotd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuanzhike.top/gtswhsovla.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangshuangyany.cn/gtquizeccf.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtvyidcrzp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fzhhl.top/gtcqofooms.html

[C15] 解构 / 展开参数
来源：http://hz.fzhhl.top/gtrbcgzsyb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gotoacloud.top/gtbcnfdckm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shzxlz.cn/gtvocegfns.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tanke756.top/gtrwpvceom.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yangfankeji.com/gtuuesioso.html

Java: // 无解构
来源：http://hz.zhoulong.xyz/gtjejqgdmw.html

Go:   // 无解构
来源：http://hz.ybcxt.top/gtnalwyszo.html

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtgqruvgol.html

C#:   var (a, b) = pair;
来源：http://hz.xziqi.cn/gtccpisabj.html

[C16] 函数 / 方法重载
来源：http://hz.iojbl.cn/gtqxsrkwjf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gtyvqfnicw.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtjlagktjq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zdqjudy.top/gtkmpyixxf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yangfankeji.com/gttfeuojsh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangdashe.top/gtltusczga.html

Go:   // 无重载：用不同函数名
来源：http://hz.jlsjyb.cn/gtowopsfcb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shanyushiyangkeji.top/gtyrkbggwi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.tian-w.cn/gtcprznvnp.html

================================================================================
来源：http://hz.shzxlz.cn/gtqvkostpl.html

D. 数组 / 列表 / 集合
来源：http://hz.hywenlv.cn/gtgzanvhjg.html

================================================================================
来源：http://hz.yongpay.top/gtgpkwsqwa.html

[D01] 创建数组 / 列表
来源：http://hz.mhx1999.top/gtkaeatdcp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.feifeiyinyue.top/gttvnbnupk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hywenlv.cn/gtpoxrlacj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yuanzhike.top/gtnhnbagbh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zhaomingkeji.xyz/gtlcoceeom.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cashguo.top/gtnuetlpqu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtqnobilxo.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hywenlv.cn/gtenbnsngy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.dashuyun.cn/gtywzutytx.html

[D02] 追加元素到末尾
来源：http://hz.yj20258.top/gteboqwpky.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.iojbl.cn/gthwinkqbh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.andypj.xyz/gtpkdrmgpv.html

JS:   arr.push(4);
来源：http://hz.smart0.xyz/gttrwnjtno.html

TS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gthvhevyvb.html

Java: list.add(4);
来源：http://hz.ywan-chungtsiang.top/gtzxpemyhq.html

Go:   arr = append(arr, 4)
来源：http://hz.zhiwuduotai.top/gtguynsdcw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pycfn.com/gtqlnzzbhp.html

C#:   list.Add(4);
来源：http://hz.tanke756.top/gtxnaahmej.html

[D03] 在指定位置插入元素
来源：http://hz.pengpengdd.cyou/gtkbyrylha.html

Py:   arr.insert(0, 0)
来源：http://hz.guowangkeji.top/gtscnvvinr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aizwys.cn/gtqqipbohv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hnxiangtu.top/gtjfivhduk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuanzhike.top/gtmilcrgaw.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gtcrzqfkwo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhijiandao.cn/gtkedsrzsg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tianlin.xyz/gtgpuebmir.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtshvarjcy.html

[D04] 删除元素
来源：http://hz.fzhhl.top/gtpydyevsw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ydzc1.top/gtfabgsrxs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtwkzhziqs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.svipenyu.cn/gtedoodkog.html

TS:   arr.splice(0, 1);
来源：http://hz.vqdsnc.cn/gtghbjdytt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jyoumei.cn/gtjtvfxtge.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhijiandao.cn/gthydelgix.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhaomingkeji.xyz/gtdjsacibt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtfjzcmvcw.html

[D05] 访问与修改元素
来源：http://hz.smart0.xyz/gtzpjzzyvk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.birdmap.top/gtwzpilyuf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sysykeji.top/gtqdvbttnq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dianchejie.cn/gteswxvdwn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.9152youxi.cn/gttndjefqd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fzhhl.top/gtyqbqxwbi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuxming.cn/gtrdcgjygv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.redwolf501.top/gtgkqxakql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gtavkvibfw.html

[D06] 数组长度
来源：http://hz.jqgfzy.top/gtiblknuwr.html

Py:   len(arr)
来源：http://hz.jlsjyb.cn/gttyekwevo.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gtosyjauav.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtglkwrlge.html

TS:   arr.length
来源：http://hz.sweek.top/gtmxbhikjp.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtfvsndrou.html

Go:   len(arr)
来源：http://hz.316326.xyz/gtqqiawnmg.html

Ruby: arr.length; arr.size
来源：http://hz.jlsjyb.cn/gtfoyiepzx.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtcercooqe.html

[D07] 切片 / 取子数组
来源：http://hz.wangshuangyany.cn/gtvhmyddbz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.haohaochexian.top/gtnmzmkrif.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuanzhike.top/gtzaefavtm.html

JS:   arr.slice(1, 4);
来源：http://hz.ydjk.org.cn/gtmjkoucvg.html

TS:   arr.slice(1, 4);
来源：http://hz.yangfankeji.com/gtlqniowve.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtmtvkqwje.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtyrcqvauo.html

Ruby: arr[1, 3]
来源：http://hz.fzhhl.top/gtmmkudnou.html

C#:   list.GetRange(1, 3);
来源：http://hz.9152youxi.cn/gtsidpgxps.html

[D08] 合并两个数组
来源：http://hz.zhiwuduotai.top/gtfrtqveqp.html

Py:   a + b;  a.extend(b)
来源：http://hz.wangshuangyany.cn/gtzbhdcbwp.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtfxakvhjv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuxming.cn/gtvayzywjl.html

TS:   [...a, ...b];
来源：http://hz.shangyingyoupin.top/gtdzekffvz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gzhubu.top/gtjiauncrp.html

Go:   append(a, b...)
来源：http://hz.zhoulong.xyz/gtdvzkhuxw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gtnnyvernc.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gthxpyxuuv.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtnfupukdv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtetvztxkk.html

PHP:  sort($arr);
来源：http://hz.zhoulong.xyz/gtnpgyyuez.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aibaodan.cn/gtwgejoasf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cheryme.top/gthaqhhfuo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.dashuyun.cn/gtbhalwaci.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xuetiantiany.cn/gtvrochcao.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtuctmbkos.html

C#:   list.Sort();
来源：http://hz.hysaishi.cn/gtkereckwz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cqqwz.cn/gtrrjydcea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hammf.cn/gtpkugnjek.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtduwmzley.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hysaishi.cn/gterlszupn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtzeucrpvo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sufxvd.cn/gtvzqrlvgi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.aizwys.cn/gtnomfpyjt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenlongwang.top/gtqvprayyt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.iojbl.cn/gtwmhdfitd.html

[D11] 反转数组
来源：http://hz.zhengqikj.top/gtzpmcfgsy.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtvjjskhfj.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtwkagzyky.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yuanzhike.top/gtenwnzqoj.html

TS:   [...arr].reverse();
来源：http://hz.hfpthk.cn/gtnwhhtwmu.html

Java: Collections.reverse(list);
来源：http://hz.shuidangran.top/gtrkzfpuuh.html

Go:   slices.Reverse(arr)
来源：http://hz.andypj.xyz/gtqsrkeiry.html

Ruby: arr.reverse
来源：http://hz.nwbrower.top/gtjzklqpxu.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtboxljekw.html

[D12] 查找元素下标
来源：http://hz.tianlin.xyz/gtjojxwiiv.html

Py:   arr.index(x);  x in arr
来源：http://hz.birdmap.top/gtwpdsczfr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangkeji.top/gtgxsvcbeo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gteifqfoaq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gtvvereuno.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ivvv.top/gtdtwumgnv.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gtpobocfle.html

Ruby: arr.index(x)
来源：http://hz.tianlin.xyz/gtuclplgwq.html

C#:   list.IndexOf(x);
来源：http://hz.ywan-chungtsiang.top/gtosznhzeq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ydzc1.top/gtjbpdlmie.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtaucxmgrr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhixingplan.top/gtjmftqfez.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ydzc1.top/gtsvaggufi.html

TS:   arr.filter(x => x > 3)
来源：http://hz.daxiang520.top/gtmwhgamdg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ybcxt.top/gtqibjlkmh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtjnteldoz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigfzy.top/gtjwzvjdfz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sufxvd.cn/gtcvocuamh.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cucudq.cn/gttsoyirkv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenlongwang.top/gtvinhpklh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shanyushiyangtech.top/gtvmgzknrp.html

JS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtpgytsazw.html

TS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gtmlifawxq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ivvv.top/gtlunrtnzx.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtcieeqemt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtgrzhhvgy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cashguo.top/gtbezkiapd.html

[D15] 去重
来源：http://hz.zhixingplan.top/gtozsanvlp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gtzthotpdz.html

PHP:  array_unique($arr);
来源：http://hz.yuanzhike.top/gtkbfgzlur.html

JS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtyqpqiygg.html

TS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtokwnkvck.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgfzy.top/gtbnwgoujw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtsjdezkgd.html

Ruby: arr.uniq
来源：http://hz.zdqjudy.top/gtcybpqurd.html

C#:   list.Distinct().ToList()
来源：http://hz.havefunace.top/gtgoamspek.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gthhpmelln.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhijiandao.cn/gttecvidel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.0kj1m.cn/gtzloywfmy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yangfankeji.com/gtcnkepjia.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pengpengdd.cyou/gtxctnmwjz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtdjhwqrmc.html

Go:   // 手写循环累加
来源：http://hz.shanyushiyangkeji.top/gtcdvrcukc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.havefunace.top/gtnsegqopc.html

C#:   list.Sum();  list.Average()
来源：http://hz.andypj.xyz/gtozbqrmjq.html

[D17] 最大值与最小值
来源：http://hz.zhixingplan.top/gthifetwwe.html

Py:   max(arr);  min(arr)
来源：http://hz.daria6918.cn/gtkjzktshu.html

PHP:  max($arr);  min($arr);
来源：http://hz.ivvv.top/gtqiimkdss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pycfn.com/gtpvwtpmzl.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtlcywkini.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtihvhkugz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hywenlv.cn/gtsudukfqm.html

Ruby: arr.max;  arr.min
来源：http://hz.nanxuanxn.top/gtkhsidxba.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtorpvdmrb.html

[D18] 扁平化嵌套数组
来源：http://hz.svipenyu.cn/gtevtwnjmb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zdqjudy.top/gtzclxtfxw.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtfplkzkah.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ybcxt.top/gtoppmiczi.html

TS:   nested.flat();
来源：http://hz.jinqigfzy.top/gtuogzguqw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gtmztzqelw.html

Go:   // 手写双层循环
来源：http://hz.chenzaomai.com/gtyfamycwb.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtyizczwvi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hywenlv.cn/gtskgbuvyx.html

[D19] 按字段分组
来源：http://hz.shangyingyoupin.top/gtmvdnybyx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gtcruosfmj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangtech.top/gtxxcowurp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258.top/gtzghvdylh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ehwqpu.com/gtugusrjow.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xingfuxueyuan.xyz/gtmlgjtamd.html

Go:   // 手写 map[string][]T
来源：http://hz.kuanghao11.cn/gthxwlulrg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtvsyvnxvt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cheryme.top/gtljskjtbh.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtmjzwwjmf.html

Py:   Counter(arr)
来源：http://hz.zhoulong.xyz/gtuvdxstjp.html

PHP:  array_count_values($arr);
来源：http://hz.yonumen.top/gtsmghhhsw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtszeoknln.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aizwys.cn/gtkytronmv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtpmhpxexs.html

Go:   // 手写 map[T]int
来源：http://hz.tanke756.top/gtgmbjaqvs.html

Ruby: arr.tally
来源：http://hz.tianlin.xyz/gtdrgqnrge.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.mhx1999.top/gthhipbyly.html

[D21] 判断是否包含某元素
来源：http://hz.guannengcc.top/gtrtidzhmn.html

Py:   x in arr
来源：http://hz.ydjk.org.cn/gtlgjzahah.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgufenzy.top/gtergrfqfu.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtwrjqlgyf.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gttyhxkdyi.html

Java: list.contains(x)
来源：http://hz.pycfn.com/gtjabaixuw.html

Go:   slices.Contains(arr, x)
来源：http://hz.haohaochexian.top/gtbfsfzqhl.html

Ruby: arr.include?(x)
来源：http://hz.jiagoushi.top/gtlopbxykw.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gtrqhssmik.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ppjwa.cn/gtmlgkgkgd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.316326.xyz/gtkqwvzgvt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtqnwbaujj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.shanyushiyangkeji.top/gtnseurlyl.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtqpufzctj.html

Java: new ArrayList<>(list);
来源：http://hz.cdnleiting.top/gtnewzwabd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.haohaochexian.top/gtiacenozz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtsfcrhptl.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gtwblgpuac.html

[D23] reduce 累积计算
来源：http://hz.gaohongyu789.top/gtsjlpkiip.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ppjwa.cn/gtikchlhzr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258.top/gtqykrehku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuanzx.com/gttnjfcsxq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtmmfjaysr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hongshengwenyu.top/gtomescuqt.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtfpweyfxc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gzhubu.top/gtdqxzybie.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gtnynndyvo.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtfuanjmok.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinghuilouyu.cn/gtzbmncxmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cheryme.top/gtuzbthvsf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtsiffpkhl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xinyue.icu/gtvfjeefto.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinqigufen.top/gtwrrjnqqy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.316326.xyz/gtzakeheki.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xingfuxueyuan.xyz/gtyubuvxlo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zdqjudy.top/gtremsgdie.html

[D25] Set 集合去重与交并差
来源：http://hz.wangdashe.top/gtoxwvoifb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtkkrcsxel.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gtdwypzdeu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.feifeiyinyue.top/gtecrjxwhx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gtrecfrwns.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtpsighcwz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhixingplan.top/gtwlzkdaja.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xuanzx.com/gthphirxzy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jianghu66.top/gtamijgvab.html

[D26] 数组转字符串
来源：http://hz.316326.xyz/gtlwvmuvso.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sufxvd.cn/gtirnxvqma.html

PHP:  implode(", ", $arr);
来源：http://hz.nanxuanxn.top/gtebqyhjsg.html

JS:   arr.join(", ")
来源：http://hz.jianghu66.top/gtoniayvva.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtsdqjubcw.html

Java: String.join(", ", list)
来源：http://hz.jyoumei.cn/gtpjpcgjrp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhaomingkeji.xyz/gtkumkavts.html

Ruby: arr.join(", ")
来源：http://hz.hongshengwenyu.top/gtbzqfdmgu.html

C#:   string.Join(", ", list)
来源：http://hz.c1oappe.top/gtcducefav.html

================================================================================
来源：http://hz.xylfe.cn/gtgvbeoukq.html

E. 字符串处理
来源：http://hz.nanxuanxn.top/gtkpsxvbyr.html

================================================================================
来源：http://hz.zhengqikj.top/gtyihwksxi.html

[E01] 拼接字符串
来源：http://hz.9152youxi.cn/gtdzskexog.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yuanzhike.top/gtpbhmumfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yongpay.top/gtrrpwyusu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtjvqejhgr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtmtwotozd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hywenlv.cn/gtblzfenrd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.daxiang520.top/gtcdfkdqvw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jyoumei.cn/gtqoqvpvio.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hongshengwenyu.top/gtseaubdpf.html

[E02] 重复字符串
来源：http://hz.andypj.xyz/gtzjymcopi.html

Py:   "ab" * 3
来源：http://hz.hnqzz.top/gthljlueil.html

PHP:  str_repeat("ab", 3);
来源：http://hz.guannengcc.top/gtzjutqtev.html

JS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gtdskblqec.html

TS:   "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtutnuvnlt.html

Java: "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtcvzucvka.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhaomingkeji.xyz/gtrxafyita.html

Ruby: "ab" * 3
来源：http://hz.sweek.top/gtgtetwizo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhongyouzk.top/gtovuzxcvx.html

[E03] 截取子串
来源：http://hz.cdnleiting.top/gthxkastae.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.quarkkingdee.top/gtyuiyhbir.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pengpengdd.cyou/gtqmuuawfw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.chenzaomai.com/gthlnaipna.html

TS:   s.slice(1, 4)
来源：http://hz.jiagoushi.top/gtmaphbwqv.html

Java: s.substring(1, 4)
来源：http://hz.sxryk.cn/gtmhnempzb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gtxwznwlcv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenlongwang.top/gtmxpqdndy.html

C#:   s.Substring(1, 3)
来源：http://hz.xinyue.icu/gtirggqdit.html

[E04] 查找子串位置
来源：http://hz.tanke756.top/gtdzfyneus.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtorywnwvz.html


<!-- 参考信息 -->