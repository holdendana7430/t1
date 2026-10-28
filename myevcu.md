代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtcxytktve.html

Go:   func add(a, b int) int
来源：http://hz.aizwys.cn/gtesxuavkx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.feifeiyinyue.top/gtiyuehfyt.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gttdbuwjdv.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gtrvmrcefz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.guowangkeji.top/gtljyidpmx.html

PHP:  // 无泛型
来源：http://hz.guannengcc.top/gtuoswvrbm.html

JS:   // 无泛型
来源：http://hz.vqdsnc.cn/gtgdixkzhz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gteaqwxgxe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.9152youxi.cn/gtuzkocekf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gteygxznqp.html

Ruby: # 无泛型
来源：http://hz.aibaodan.cn/gtsjapvmuk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sweek.top/gtfcbobgel.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtgfnbtuus.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.hnxiangtu.top/gtcjzniiuh.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hongshengwenyu.top/gtoxtuzxcf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cqqwz.cn/gtfosrutwy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhixingplan.top/gtqemrjftb.html

Java: // 无解构
来源：http://hz.chenzaomai.com/gtlmkzosbh.html

Go:   // 无解构
来源：http://hz.yuanzhike.top/gteeafbnnv.html

Ruby: a, b = pair
来源：http://hz.xuetiantiany.cn/gthlkiqshb.html

C#:   var (a, b) = pair;
来源：http://hz.chenlongwang.top/gtydowpryr.html

[C16] 函数 / 方法重载
来源：http://hz.hnqzz.top/gthunhwdfn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cashguo.top/gtnfyrqvmx.html

PHP:  // 无重载
来源：http://hz.ydjk.org.cn/gtjytvurba.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hysaishi.cn/gtboyupwyz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.316326.xyz/gtxgljrzom.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuanzhike.top/gthpqkeizy.html

Go:   // 无重载：用不同函数名
来源：http://hz.zdqjudy.top/gtnaghfapf.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cqqwz.cn/gtatfunxqe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.sysykeji.top/gtvqsrhlqr.html

================================================================================
来源：http://hz.cdnleiting.top/gtxgwaxkwa.html

D. 数组 / 列表 / 集合
来源：http://hz.yueranfly.top/gtewpaaida.html

================================================================================
来源：http://hz.guannengcc.top/gtjjdudtkj.html

[D01] 创建数组 / 列表
来源：http://hz.zhoulong.xyz/gtoccelvvc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.quarkkingdee.top/gtomnobrby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xylfe.cn/gtlutwcoqy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.snrcjt.cn/gtjumyncaw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gttkjjeked.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtlphsqhau.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtnlmjtpik.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinghuilouyu.cn/gtyzcqoluy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jyoumei.cn/gtabvtrhns.html

[D02] 追加元素到末尾
来源：http://hz.yj20258888.top/gtywqgumff.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yonumen.top/gtzewjtgdb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cashguo.top/gtrkjkfbej.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gttbvclkqq.html

TS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtjnmflqhx.html

Java: list.add(4);
来源：http://hz.pengpengdd.cyou/gtjqwarukd.html

Go:   arr = append(arr, 4)
来源：http://hz.cucudq.cn/gtflhpqnhn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gtzpwwlttt.html

C#:   list.Add(4);
来源：http://hz.zhiwuduotai.top/gtahwkzhxc.html

[D03] 在指定位置插入元素
来源：http://hz.jianghu66.top/gtbywzcaes.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtpqyieqqe.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.shanyushiyangtech.top/gtbidautxg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nwbrower.top/gtgiuvhpsl.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtlgdbfops.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gttnztfsec.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.snrcjt.cn/gtryotcjnb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cashguo.top/gtswcletro.html

C#:   list.Insert(0, 0);
来源：http://hz.ehwqpu.com/gtcrpwptmz.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtptkxlcgk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.9152youxi.cn/gtbftxevnu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hywenlv.cn/gtwxytfhuw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtwpqnibjc.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtqwqghpsp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yongpay.top/gtrajzwayq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cdnleiting.top/gtpktinzjw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj202588.top/gtgrknbbvc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jiagoushi.top/gtrpdkirgr.html

[D05] 访问与修改元素
来源：http://hz.ybcxt.top/gtqipaazpj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258888.top/gtcgqdsgyl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtdecmzqkm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenlongwang.top/gtihqvccnz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yuxming.cn/gtpghegbns.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.birdmap.top/gtwyrxpalj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yvedp.cn/gtvfyzrjaf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guannengcc.top/gtvwpwydoo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtbxqdbgts.html

[D06] 数组长度
来源：http://hz.daria6918.cn/gtdhitohhe.html

Py:   len(arr)
来源：http://hz.yvedp.cn/gtxrjqojaz.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtrikkhucj.html

JS:   arr.length
来源：http://hz.chenzaomai.com/gttkwpgevu.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtzrfglxva.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtmbllbaxr.html

Go:   len(arr)
来源：http://hz.kuanghao11.cn/gtavvpmekn.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gthzamyvjp.html

C#:   list.Count;
来源：http://hz.ydzc1.top/gtpvilbskh.html

[D07] 切片 / 取子数组
来源：http://hz.ydzc1.top/gtfiqaepja.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinyuanbaomall.cn/gtxswvyeog.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.pengpengdd.cyou/gttkfzulcs.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtrdqemqis.html

TS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtuqkdpkas.html

Java: list.subList(1, 4);
来源：http://hz.sxryk.cn/gtohzpikvf.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtmaehcaoa.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtpndcxzen.html

C#:   list.GetRange(1, 3);
来源：http://hz.gzhubu.top/gtpyzsnptl.html

[D08] 合并两个数组
来源：http://hz.hnxiangtu.top/gtlexcrgcd.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhijiandao.cn/gtfalpqpyt.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtwocwhcng.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.iojbl.cn/gtfgssebnq.html

TS:   [...a, ...b];
来源：http://hz.zhengqikj.top/gtnfehqqis.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtvamxvkqt.html

Go:   append(a, b...)
来源：http://hz.ivvv.top/gtagodyziy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtfteiyysv.html

C#:   a.Concat(b).ToList()
来源：http://hz.ivvv.top/gtcrefasrs.html

[D09] 排序（升序）
来源：http://hz.cheryme.top/gtttivvmwv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigfzy.top/gtchtxvhvi.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtzfdltzap.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fzhhl.top/gtgquqmgkm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hysaishi.cn/gtuyofynna.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gtfhwzzvjz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gogol.net.cn/gtzdhbgjcm.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtpjybnvew.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gttrflkykk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.ywan-chungtsiang.top/gtgthunqew.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuetiantiany.cn/gtcffotcrz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtdhmcakfq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtqpwuvaua.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtxyyyznfc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.vqdsnc.cn/gtbasuiigm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hnxiangtu.top/gtluyamexm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.quarkkingdee.top/gtzjzqcxvb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ywan-chungtsiang.top/gtdbequdkq.html

[D11] 反转数组
来源：http://hz.birdmap.top/gtzdliurkr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtaklmiwiw.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtuvkbyjhp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.wangshuangyany.cn/gtdwyretlu.html

TS:   [...arr].reverse();
来源：http://hz.nanxuanxn.top/gtmnkcsybw.html

Java: Collections.reverse(list);
来源：http://hz.cashguo.top/gtovsqbkgy.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtxepfzabx.html

Ruby: arr.reverse
来源：http://hz.chenjidiqi.icu/gtrczsuzhy.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtdxnzytnk.html

[D12] 查找元素下标
来源：http://hz.zdqjudy.top/gtnqqjheby.html

Py:   arr.index(x);  x in arr
来源：http://hz.ehwqpu.com/gtxphvmfaj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yangfankeji.com/gtvlcwhdfd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtkfmnifxq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtqfdcjwqv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtqioilhjc.html

Go:   slices.Index(arr, x)
来源：http://hz.yvedp.cn/gtsomqmako.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtfljuqddt.html

C#:   list.IndexOf(x);
来源：http://hz.haohaochexian.top/gtjzupymae.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtbqeixsze.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.52xcode.cn/gtklyrbilc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxinkj.top/gtkgfqyslp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtcteqmdvs.html

TS:   arr.filter(x => x > 3)
来源：http://hz.aibaodan.cn/gtpmpxgpnh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jiagoushi.top/gtphxbogmt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xziqi.cn/gtvpuwwpjh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.aizwys.cn/gtkosquowp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtujtnhndk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yongpay.top/gtycjmzexw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hnqzz.top/gtqfvsttut.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.snrcjt.cn/gthgfpftvg.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtydndiyns.html

TS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtsofhbcwc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gaohongyu789.top/gtrtrncehp.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtjbtmcoel.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtinzxgoeq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.iojbl.cn/gtdkyjnezi.html

[D15] 去重
来源：http://hz.jiagoushi.top/gtfcmqkzve.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.meibo888.top/gtgguteske.html

PHP:  array_unique($arr);
来源：http://hz.gogol.net.cn/gtqohhnmzz.html

JS:   [...new Set(arr)]
来源：http://hz.yongpay.top/gtmbzjheuu.html

TS:   [...new Set(arr)]
来源：http://hz.yj202588.top/gtobegfvjs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.andypj.xyz/gtltywuzxj.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtrlkqiyys.html

Ruby: arr.uniq
来源：http://hz.tian-w.cn/gtdplksgha.html

C#:   list.Distinct().ToList()
来源：http://hz.zdqjudy.top/gtkokoocyg.html

[D16] 求和与平均值
来源：http://hz.zdqjudy.top/gtxmemghus.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jyoumei.cn/gtlwbsykgm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydjk.org.cn/gtneviixzq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuetiantiany.cn/gtterbjqph.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtvlcufscz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtwpsucygx.html

Go:   // 手写循环累加
来源：http://hz.bjfxy.top/gtntwycnds.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pycfn.com/gtisuxlifn.html

C#:   list.Sum();  list.Average()
来源：http://hz.c1oappe.top/gtcgvhrpio.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gtnlbvyeef.html

Py:   max(arr);  min(arr)
来源：http://hz.nwbrower.top/gtoyautejk.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gtnahgrmzg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.shanyushiyangkeji.top/gthgabvyeu.html

TS:   Math.max(...arr);
来源：http://hz.shangyingyoupin.top/gtzjdtdlbi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sufxvd.cn/gtirtswpuv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gtvhddjdvu.html

Ruby: arr.max;  arr.min
来源：http://hz.cqqwz.cn/gtcuutbbbb.html

C#:   list.Max();  list.Min()
来源：http://hz.hammf.cn/gtcaiwwmyv.html

[D18] 扁平化嵌套数组
来源：http://hz.iojbl.cn/gtliyrqcqg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtzlfgebou.html

PHP:  array_merge(...$nested);
来源：http://hz.jinyuanbaomall.cn/gtjapihwly.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ppjwa.cn/gttckuivqy.html

TS:   nested.flat();
来源：http://hz.hfpthk.cn/gtmmiigsrq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhoulong.xyz/gtblsdfwfp.html

Go:   // 手写双层循环
来源：http://hz.zhixingplan.top/gtrruqglpp.html

Ruby: nested.flatten
来源：http://hz.yanxiufei.cn/gtpxvhcarg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhongyouzk.top/gtfsjovxxd.html

[D19] 按字段分组
来源：http://hz.yonumen.top/gtisjietyz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jqgfzy.top/gtokdrzdxv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtjvmwpmwk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ivvv.top/gtqslmbfxf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gteqlvyglm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenjidiqi.icu/gtxmjbbofs.html

Go:   // 手写 map[string][]T
来源：http://hz.cdnleiting.top/gttkryhqwb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ybcxt.top/gthstjncgk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gtjtuwcvfo.html

[D20] 统计每个元素出现次数
来源：http://hz.smart0.xyz/gtnpxujtny.html

Py:   Counter(arr)
来源：http://hz.ppjwa.cn/gtrghvqxht.html

PHP:  array_count_values($arr);
来源：http://hz.yueranfly.top/gtdrfeuzac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtjabplyjz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtkgssgcec.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtelcskheb.html

Go:   // 手写 map[T]int
来源：http://hz.zhaomingkeji.xyz/gtfrfrjxvl.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtojgwubjg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gthoipkrkn.html

[D21] 判断是否包含某元素
来源：http://hz.gaohongyu789.top/gtscxsblmd.html

Py:   x in arr
来源：http://hz.hnxiangtu.top/gtavusefii.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cqqwz.cn/gtlnbqzlcj.html

JS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtdzrstwvi.html

TS:   arr.includes(x)
来源：http://hz.jinqigufen.top/gtbyayohav.html

Java: list.contains(x)
来源：http://hz.sxryk.cn/gtxxkbwsba.html

Go:   slices.Contains(arr, x)
来源：http://hz.redwolf501.top/gtubbnwkxt.html

Ruby: arr.include?(x)
来源：http://hz.jinqigfzy.top/gtvcatqtll.html

C#:   list.Contains(x)
来源：http://hz.ybcxt.top/gtiwpqlqkh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtsppjzyld.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.havefunace.top/gtkplneawq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtlmhlofvh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtdikxnoas.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtfsrixgws.html

Java: new ArrayList<>(list);
来源：http://hz.jlsjyb.cn/gtcpxiknyp.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtthpnpnop.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yvedp.cn/gtahdcwylf.html

C#:   new List<int>(list);
来源：http://hz.jinyuanbaomall.cn/gtajscrxae.html

[D23] reduce 累积计算
来源：http://hz.chenlongwang.top/gtnincymfn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gtajtapttq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.bjfxy.top/gtaslurric.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtppgvmkfb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydjk.org.cn/gtacszlygj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gotoacloud.top/gtyzfedbig.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtkfuiyqbk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gotoacloud.top/gtcitcztbp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hnxiangtu.top/gtuugywprj.html

[D24] 字典 / Map 基本操作
来源：http://hz.xuetiantiany.cn/gtswvhtlne.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cdnleiting.top/gtqirurptg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shanyushiyangkeji.top/gthiopzekm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hnxiangtu.top/gtineoeedi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cheryme.top/gtvlwvpqez.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shzxlz.cn/gtgdytxwco.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtabqnfwyj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtsdoamnue.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtrfgqnzwh.html

[D25] Set 集合去重与交并差
来源：http://hz.jlsjyb.cn/gtwimnuaak.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtnkcfjjix.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenzaomai.com/gtczdjrxai.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dashuyun.cn/gtpzftfiyr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jyoumei.cn/gtemveesgp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gtioupjnwe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ybcxt.top/gtxfeghmjk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtntvurnzc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtwwrtpcwk.html

[D26] 数组转字符串
来源：http://hz.daria6918.cn/gtcdhlqvzh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cashguo.top/gtgabffkwq.html

PHP:  implode(", ", $arr);
来源：http://hz.redwolf501.top/gtioczbsch.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtshqihlge.html

TS:   arr.join(", ")
来源：http://hz.jinqigufen.top/gtlljtspya.html

Java: String.join(", ", list)
来源：http://hz.chenzaomai.com/gtrodppxxr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gttbiwtwmh.html

Ruby: arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtvxumszwi.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtlxggxtit.html

================================================================================
来源：http://hz.snrcjt.cn/gtlbkiqibj.html

E. 字符串处理
来源：http://hz.jlsjyb.cn/gtlebrrukz.html

================================================================================
来源：http://hz.smart0.xyz/gtvpxbyfex.html

[E01] 拼接字符串
来源：http://hz.zdqjudy.top/gtcilbozki.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ydzc1.top/gtjojggjfx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yueranfly.top/gtcldhwnje.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtsrrogckz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tianlin.xyz/gtbsfxxpzy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xylfe.cn/gtglipbyqn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj202588.top/gtklnbhhxd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sysykeji.top/gtkzaudols.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.guowangkeji.top/gtfxnkqqli.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtntkasvuf.html

Py:   "ab" * 3
来源：http://hz.snrcjt.cn/gtmmapawmp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cheryme.top/gtyuhshlwq.html

JS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gthgevvwak.html

TS:   "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtxmkyeqdl.html

Java: "ab".repeat(3)
来源：http://hz.zhaomingkeji.xyz/gtcjjjzzly.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yonumen.top/gtvnpvlrld.html

Ruby: "ab" * 3
来源：http://hz.yuanzhike.top/gtzudrplew.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinqigfzy.top/gtbflctxky.html

[E03] 截取子串
来源：http://hz.gogol.net.cn/gtgdsbnazs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sysykeji.top/gtjzbycusd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhixingplan.top/gtapwaxqch.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.guowangkeji.top/gtemtbrcbm.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258.top/gtxtymyjuw.html

Java: s.substring(1, 4)
来源：http://hz.hammf.cn/gtewojzwia.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cucudq.cn/gtpudreend.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.pycfn.com/gtcupsrcoq.html

C#:   s.Substring(1, 3)
来源：http://hz.snrcjt.cn/gtriqzjolk.html

[E04] 查找子串位置
来源：http://hz.hywenlv.cn/gtxgzddpkt.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cucudq.cn/gtgdyhdhwb.html


<!-- 参考信息 -->