代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtyeofjbkw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jiagoushi.top/gtpqqgfusd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ivvv.top/gtlxecczdz.html

Ruby: # 无泛型
来源：http://hz.cqqwz.cn/gtrteipldu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gthhgnlezq.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtbxkqlrff.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xingfuxueyuan.xyz/gtyoejeoyb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtxqpdoxof.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xuetiantiany.cn/gthhslucmw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxinkj.top/gtihedyanc.html

Java: // 无解构
来源：http://hz.pengpengdd.cyou/gtnlbgzlpj.html

Go:   // 无解构
来源：http://hz.jinqigfzy.top/gtvfqhccbt.html

Ruby: a, b = pair
来源：http://hz.bjfxy.top/gthvmmaddy.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtyfevlvlo.html

[C16] 函数 / 方法重载
来源：http://hz.smart0.xyz/gtontxsquk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gtiahjewoq.html

PHP:  // 无重载
来源：http://hz.jianghu66.top/gtdzhbsdvu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtcxaqsgnf.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guowangkeji.top/gtjpgcakiy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtbbmlpjed.html

Go:   // 无重载：用不同函数名
来源：http://hz.jqgufenzy.top/gtuggsflyq.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxinkj.top/gtbsggghbu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daxiang520.top/gtpbidgdrt.html

================================================================================
来源：http://hz.pycfn.com/gtorwcyjjl.html

D. 数组 / 列表 / 集合
来源：http://hz.sufxvd.cn/gtmsgpshlt.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsjkqpdwq.html

[D01] 创建数组 / 列表
来源：http://hz.tian-w.cn/gtvighlslp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangkeji.top/gtqdmmtbpl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.nanxinkj.top/gtwpjzmepi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ydzc1.top/gtfvvgdbts.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jyoumei.cn/gtvrmdkyps.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jlsjyb.cn/gtelqcxvhn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydzc1.top/gtecdobdhs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gtsntuhgnr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zycfv.cn/gtbvwsobhd.html

[D02] 追加元素到末尾
来源：http://hz.zhiwuduotai.top/gtwijwqieb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.haohaochexian.top/gtnkhxauqr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gttrgohgse.html

JS:   arr.push(4);
来源：http://hz.shuidangran.top/gtiaeugqan.html

TS:   arr.push(4);
来源：http://hz.hammf.cn/gtqnjijedn.html

Java: list.add(4);
来源：http://hz.aizwys.cn/gtdyiilzye.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtdpyziqbu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hongshengwenyu.top/gtppsooqyq.html

C#:   list.Add(4);
来源：http://hz.zdqjudy.top/gtmqrglwri.html

[D03] 在指定位置插入元素
来源：http://hz.shzxlz.cn/gtelmfjcwt.html

Py:   arr.insert(0, 0)
来源：http://hz.quarkkingdee.top/gthsmdwjta.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtplxeysht.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sysykeji.top/gtgsfljorq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jqgufenzy.top/gtqidrvalj.html

Java: list.add(0, 0);
来源：http://hz.jqgfzy.top/gtxzpfldfn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nanxinkj.top/gtsrettong.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yongpay.top/gtmrilcqyl.html

C#:   list.Insert(0, 0);
来源：http://hz.yj202588.top/gtqymjplxe.html

[D04] 删除元素
来源：http://hz.9152youxi.cn/gttokruwlc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuanzhike.top/gtkdjfgkch.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.0kj1m.cn/gttysbzknc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.quarkkingdee.top/gttclgryvt.html

TS:   arr.splice(0, 1);
来源：http://hz.xuanzx.com/gtrhgpwcpv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.quarkkingdee.top/gttabgguxi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yueranfly.top/gtrjhgltvc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtrvjnimhg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtncfqugza.html

[D05] 访问与修改元素
来源：http://hz.c1oappe.top/gtxjdjokcu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtydbsgpjb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtzrdxxxbb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.aizwys.cn/gtgenwzzjy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gtdsgdegne.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hywenlv.cn/gtkmsogwty.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.feifeiyinyue.top/gtosoorcdd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.svipenyu.cn/gtqvqhapwg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuxming.cn/gtvtdaeeii.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtuulcnhhn.html

Py:   len(arr)
来源：http://hz.sxryk.cn/gtnetgrpzq.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtfsesnlzs.html

JS:   arr.length
来源：http://hz.yvedp.cn/gtpcowsgrz.html

TS:   arr.length
来源：http://hz.jqgufenzy.top/gtrovrkjgi.html

Java: list.size();
来源：http://hz.yonumen.top/gtoxhiwovd.html

Go:   len(arr)
来源：http://hz.daria6918.cn/gtweiilhud.html

Ruby: arr.length; arr.size
来源：http://hz.aibaodan.cn/gtknsjxpif.html

C#:   list.Count;
来源：http://hz.0kj1m.cn/gtflmsqwuq.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtirukytym.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gotoacloud.top/gtggbsrylg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.bjfxy.top/gtrtzdsjvb.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtaatbdvgo.html

TS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtmrshhuqm.html

Java: list.subList(1, 4);
来源：http://hz.ivvv.top/gtmafmpcrn.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtftqvytzr.html

Ruby: arr[1, 3]
来源：http://hz.jinqigufen.top/gtcrwphzob.html

C#:   list.GetRange(1, 3);
来源：http://hz.yvedp.cn/gtzklngofk.html

[D08] 合并两个数组
来源：http://hz.shzxlz.cn/gtwwgzgpvv.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtfhqdiiwt.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtmltigddp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.sysykeji.top/gtdijhdfjq.html

TS:   [...a, ...b];
来源：http://hz.xuanzx.com/gtzmwzjwxo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtzccoyzwl.html

Go:   append(a, b...)
来源：http://hz.jyoumei.cn/gtjxsqrbwj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daria6918.cn/gtihghsbes.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhoulong.xyz/gtqhxjyzwi.html

[D09] 排序（升序）
来源：http://hz.52xcode.cn/gtwspsytbq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gaohongyu789.top/gtvvswgfpj.html

PHP:  sort($arr);
来源：http://hz.jiagoushi.top/gtllyiugef.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cucudq.cn/gthbszutdj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gaohongyu789.top/gtjkgtukmj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.gaohongyu789.top/gtkxrhcokw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxuanxn.top/gtlyveudvy.html

Ruby: arr.sort
来源：http://hz.cashguo.top/gtdxbelgee.html

C#:   list.Sort();
来源：http://hz.sysykeji.top/gtujewxvkr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jianghu66.top/gtwhnlgzfj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.meibo888.top/gtzxpjtgqz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sysykeji.top/gtsaujeynu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtocawxaiz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtfhzvefps.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guannengcc.top/gtzfkfqgzf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zdqjudy.top/gtqcoarahe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cashguo.top/gtttgijoge.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yuanzhike.top/gtxhoxhcyl.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gttmkapsrx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yvedp.cn/gtwrhjblav.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gthlfhvxyc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gtvhtfmefy.html

TS:   [...arr].reverse();
来源：http://hz.yuanzhike.top/gtikpzkmpu.html

Java: Collections.reverse(list);
来源：http://hz.zhoulong.xyz/gtlkwkuykx.html

Go:   slices.Reverse(arr)
来源：http://hz.yvedp.cn/gtiqwmycog.html

Ruby: arr.reverse
来源：http://hz.guowangkeji.top/gtojqbnjkl.html

C#:   list.Reverse();
来源：http://hz.xuanzx.com/gtxvzkgzuu.html

[D12] 查找元素下标
来源：http://hz.yj202588.top/gtvuzwclaz.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gtjmxiuzsz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pengpengdd.cyou/gthnvmpmuc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtoenheemi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtmslehybq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gtxsdhffgv.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtcfgfeetz.html

Ruby: arr.index(x)
来源：http://hz.xuanzx.com/gtfubwygna.html

C#:   list.IndexOf(x);
来源：http://hz.ybcxt.top/gthbtrzfiz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnqzz.top/gtdccsmraf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tianlin.xyz/gtwdrdfujo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtcuxcixhq.html

JS:   arr.filter(x => x > 3)
来源：http://hz.vqdsnc.cn/gtuywxzhkt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtalwoizrk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgfzy.top/gtewcqfzon.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.andypj.xyz/gtncobjqbu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtdvjsbxya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gtvsmtkpzg.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tanke756.top/gtuhjclvbu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtjhfwzcht.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangdashe.top/gteyrlricr.html

JS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtzxcmxznk.html

TS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtnhcatyuj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.meibo888.top/gtrwodttyi.html

Go:   // 手写循环
来源：http://hz.ehwqpu.com/gtnjtacezg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtsdjcfrag.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.52xcode.cn/gtwbrujgeq.html

[D15] 去重
来源：http://hz.hammf.cn/gtzznfkzxn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gtmltotyaj.html

PHP:  array_unique($arr);
来源：http://hz.chenjidiqi.icu/gtjjytphpo.html

JS:   [...new Set(arr)]
来源：http://hz.c1oappe.top/gtjuviehzf.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtqfwkiwnd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.cashguo.top/gtdhkhqvzv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtzwzmteyd.html

Ruby: arr.uniq
来源：http://hz.smart0.xyz/gtqcquhcau.html

C#:   list.Distinct().ToList()
来源：http://hz.9152youxi.cn/gtoelrxvwd.html

[D16] 求和与平均值
来源：http://hz.tanke756.top/gthzsfdpnw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fzhhl.top/gtipqwvawe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shanyushiyangtech.top/gtwvamvrhl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtqtfxkomx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258888.top/gtbqkurfhf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ydjk.org.cn/gtdetwfezy.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtkdniadzi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.dashuyun.cn/gthsrcosvi.html

C#:   list.Sum();  list.Average()
来源：http://hz.yongpay.top/gtzjpxaiel.html

[D17] 最大值与最小值
来源：http://hz.dashuyun.cn/gtmiejuoth.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtitxqxldi.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuanzx.com/gtifkjuoug.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xinyue.icu/gtmsbfrbwa.html

TS:   Math.max(...arr);
来源：http://hz.nwbrower.top/gtpthpcngf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.svipenyu.cn/gtgyqkbqgg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj202588.top/gtbxsvruik.html

Ruby: arr.max;  arr.min
来源：http://hz.gzhubu.top/gtjkjymjnj.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtszbvyyyw.html

[D18] 扁平化嵌套数组
来源：http://hz.xuanzx.com/gtsyzmlsfq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtsbkzkyjd.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtfegeaxsw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gttmujjcdu.html

TS:   nested.flat();
来源：http://hz.aizwys.cn/gtxnrbyrgn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangtech.top/gtovnxedlb.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtjgrfhxwl.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtloyxbpmh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shangyingyoupin.top/gtcynkzyeo.html

[D19] 按字段分组
来源：http://hz.zycfv.cn/gtmcdhqiyj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gthvnwrxdj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sufxvd.cn/gtnwgmojfh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.c1oappe.top/gthwmmlzzp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtecgyfnfb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtpkqaepxn.html

Go:   // 手写 map[string][]T
来源：http://hz.pengpengdd.cyou/gtqanwuyhz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cdnleiting.top/gthpkdmbqt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dianchejie.cn/gtvichqjgq.html

[D20] 统计每个元素出现次数
来源：http://hz.chenlongwang.top/gtzdknhsgm.html

Py:   Counter(arr)
来源：http://hz.chenzaomai.com/gtaoahbmgj.html

PHP:  array_count_values($arr);
来源：http://hz.havefunace.top/gtpsficaqp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.316326.xyz/gtizeipuoe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sxryk.cn/gtxpgoqgcm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhoulong.xyz/gtjfrcjsgt.html

Go:   // 手写 map[T]int
来源：http://hz.hnqzz.top/gtybzhmxor.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtlvdtlkqi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xingfuxueyuan.xyz/gtxluwybtc.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtntroknls.html

Py:   x in arr
来源：http://hz.316326.xyz/gtwyuuansj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nanxuanxn.top/gtjxxythzz.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtpjbmxymd.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtwasjriwi.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtgkzwgety.html

Go:   slices.Contains(arr, x)
来源：http://hz.hongshengwenyu.top/gtiefweyjj.html

Ruby: arr.include?(x)
来源：http://hz.yj20258.top/gtccblapvb.html

C#:   list.Contains(x)
来源：http://hz.xuanzx.com/gtqdjwvyfh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtlhftrywb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258.top/gttmeagixg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ywan-chungtsiang.top/gtktlmgtol.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.dashuyun.cn/gtjdxkaycu.html

TS:   [...arr];
来源：http://hz.andypj.xyz/gthryggljt.html

Java: new ArrayList<>(list);
来源：http://hz.nanxinkj.top/gtqmlntlun.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.316326.xyz/gtwrijycqb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sysykeji.top/gtqjlfxiyj.html

C#:   new List<int>(list);
来源：http://hz.yj20258.top/gtvtocfsuf.html

[D23] reduce 累积计算
来源：http://hz.jianghu66.top/gtmgslljbs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenjidiqi.icu/gtlhhrxsyr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtxrszxjwy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hammf.cn/gtufldlifb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtwlbbohqi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daria6918.cn/gtisxmpivp.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtibiopsqi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.xziqi.cn/gtujoncvyj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hysaishi.cn/gtdcvdkruv.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhoulong.xyz/gtjjmpnyll.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinyuanbaomall.cn/gtmubgbwjz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenjidiqi.icu/gttonvybjf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtarkhmege.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fengsongda.top/gtwyczpnnh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.316326.xyz/gttadyiqlb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zdqjudy.top/gtfqjkcdxs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangdashe.top/gtkxqkmozy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dashuyun.cn/gtuiwstdwn.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtfnkvwywr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.gaohongyu789.top/gtmpvivsny.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtqfphwjew.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.haohaochexian.top/gtqyomynbg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.c1oappe.top/gttonqeqeu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yj20258.top/gtqfespkld.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cdnleiting.top/gtminibaer.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.iojbl.cn/gtaftkvzus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xinyue.icu/gtjorxlyzx.html

[D26] 数组转字符串
来源：http://hz.zhixingplan.top/gtewgwoytu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tanke756.top/gtcubynbcz.html

PHP:  implode(", ", $arr);
来源：http://hz.yvedp.cn/gtstsazmga.html

JS:   arr.join(", ")
来源：http://hz.feifeiyinyue.top/gtbojikeav.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtkxodeoed.html

Java: String.join(", ", list)
来源：http://hz.jqgufenzy.top/gtlssbjljv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gogol.net.cn/gtfzmhbucv.html

Ruby: arr.join(", ")
来源：http://hz.vqdsnc.cn/gtizculnzt.html

C#:   string.Join(", ", list)
来源：http://hz.daxiang520.top/gtacjcptll.html

================================================================================
来源：http://hz.jiagoushi.top/gtqybstxgj.html

E. 字符串处理
来源：http://hz.chenlongwang.top/gtvluprwho.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtzyrhlutf.html

[E01] 拼接字符串
来源：http://hz.xylfe.cn/gtpbpukwln.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtvmuqaobp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.wangdashe.top/gtanuxdcdh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.havefunace.top/gtcttvvdzw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gtmowpnsva.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhaomingkeji.xyz/gtfrcbhhxt.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhengqikj.top/gtddgewhub.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jiagoushi.top/gtwnucwpbq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.feifeiyinyue.top/gtvelbnknl.html

[E02] 重复字符串
来源：http://hz.sufxvd.cn/gtpddpcset.html

Py:   "ab" * 3
来源：http://hz.pengpengdd.cyou/gthhtwzfle.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xinyue.icu/gtcljwioat.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtjwqjesxi.html

TS:   "ab".repeat(3)
来源：http://hz.yuanzhike.top/gtbkjpijyh.html

Java: "ab".repeat(3)
来源：http://hz.gogol.net.cn/gthmyvwitj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shanyushiyangtech.top/gtuwtsxlfw.html

Ruby: "ab" * 3
来源：http://hz.guowangkeji.top/gtcglcvnjk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.316326.xyz/gteoykrkri.html

[E03] 截取子串
来源：http://hz.chenzaomai.com/gthalbmdgg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydzc1.top/gtlqcvzxyb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigfzy.top/gtxhkxivfb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gotoacloud.top/gtqivwtjpb.html

TS:   s.slice(1, 4)
来源：http://hz.wangdashe.top/gtipxfonvm.html

Java: s.substring(1, 4)
来源：http://hz.ppjwa.cn/gthlynadfl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.316326.xyz/gtiqgziulh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jiagoushi.top/gtvrujgrje.html

C#:   s.Substring(1, 3)
来源：http://hz.zhaomingkeji.xyz/gtjhydugcd.html

[E04] 查找子串位置
来源：http://hz.jinqigufen.top/gtyimoqcur.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenjidiqi.icu/gtpogfnxmg.html

PHP:  strpos($s, "x");
来源：http://hz.yj20258888.top/gteahozfim.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.feifeiyinyue.top/gtoayokvmv.html

TS:   s.indexOf("x")
来源：http://hz.haohaochexian.top/gtmuvxlllg.html

Java: s.indexOf("x")
来源：http://hz.svipenyu.cn/gtkanrczub.html

Go:   strings.Index(s, "x")
来源：http://hz.svipenyu.cn/gtffortveq.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gtyvmtrlus.html

C#:   s.IndexOf("x")
来源：http://hz.nanxuanxn.top/gtjrigbcez.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.quarkkingdee.top/gtvwotdnbd.html


<!-- 参考信息 -->