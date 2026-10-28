代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.sweek.top/gtgjuxsrwx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.vqdsnc.cn/gtyyhghtbt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenlongwang.top/gtutizilkw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtginvletb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cucudq.cn/gtguenicsr.html

Go:   func add(a, b int) int
来源：http://hz.sufxvd.cn/gthuvtxgsj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.iojbl.cn/gtbvtbffky.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aibaodan.cn/gtkarwnmnx.html

[C14] 泛型函数
来源：http://hz.yangfankeji.com/gtoeewrusc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinqigfzy.top/gtyfjapdxx.html

PHP:  // 无泛型
来源：http://hz.tian-w.cn/gtsgcwjhet.html

JS:   // 无泛型
来源：http://hz.yj20258888.top/gtifoxlnvh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.aizwys.cn/gtnvfotxtx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yangfankeji.com/gtkzvkqwkt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenjidiqi.icu/gtrjkrmxwy.html

Ruby: # 无泛型
来源：http://hz.yj20258888.top/gtwiaubald.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jqgufenzy.top/gtymftzguc.html

[C15] 解构 / 展开参数
来源：http://hz.dianchejie.cn/gtoxmkvmvi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gtgkaijssb.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xingfuxueyuan.xyz/gtqlbsftmd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xylfe.cn/gtfokmoaql.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtxxingzdr.html

Java: // 无解构
来源：http://hz.fzhhl.top/gtfhbjuvam.html

Go:   // 无解构
来源：http://hz.tianlin.xyz/gterjckmnd.html

Ruby: a, b = pair
来源：http://hz.wangdashe.top/gtagzgleqz.html

C#:   var (a, b) = pair;
来源：http://hz.zhiwuduotai.top/gtujlupjvg.html

[C16] 函数 / 方法重载
来源：http://hz.andypj.xyz/gtlvokaxbm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnxiangtu.top/gtyjadwege.html

PHP:  // 无重载
来源：http://hz.cashguo.top/gtbcnlxdhp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxinkj.top/gtbbobkkxw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.0kj1m.cn/gtzxhrzjfk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gtnwpprugv.html

Go:   // 无重载：用不同函数名
来源：http://hz.daxiang520.top/gtdauukqip.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ppjwa.cn/gtgivgpzxq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nanxinkj.top/gtmpayykbq.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnmwyyavv.html

D. 数组 / 列表 / 集合
来源：http://hz.ydzc1.top/gtbnmlqgdz.html

================================================================================
来源：http://hz.yvedp.cn/gtushvhdme.html

[D01] 创建数组 / 列表
来源：http://hz.shanyushiyangkeji.top/gtbbuwdpyz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hywenlv.cn/gtbxmybqca.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.shanyushiyangtech.top/gtbdrcmpei.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.havefunace.top/gthwbpxait.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangtech.top/gtskpqvttq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuxming.cn/gtyfhnznem.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jinqigufen.top/gtoldrdfft.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hfpthk.cn/gtvmpkafum.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtfewmmcfl.html

[D02] 追加元素到末尾
来源：http://hz.fzhhl.top/gtrnjhopnn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgfzy.top/gtzxzqnwuw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shangyingyoupin.top/gtumkpsejq.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtznqpynxb.html

TS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtnziozhhc.html

Java: list.add(4);
来源：http://hz.chenzaomai.com/gtvencxvfv.html

Go:   arr = append(arr, 4)
来源：http://hz.jlsjyb.cn/gtokfafbna.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtbnoenhcy.html

C#:   list.Add(4);
来源：http://hz.wangshuangyany.cn/gtnechzhzw.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gtokwjjqyd.html

Py:   arr.insert(0, 0)
来源：http://hz.sysykeji.top/gtxcvtboey.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgufenzy.top/gtqbtxhqzl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zycfv.cn/gtqhhrskyp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtgpvruwuv.html

Java: list.add(0, 0);
来源：http://hz.dianchejie.cn/gtyaeydviu.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnqzz.top/gtrpmradfh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.xuetiantiany.cn/gtswdjbxpy.html

C#:   list.Insert(0, 0);
来源：http://hz.xuetiantiany.cn/gtrnzfzhcj.html

[D04] 删除元素
来源：http://hz.cheryme.top/gtrifomgom.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.iojbl.cn/gthhotbrvn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tianlin.xyz/gtkzhotgne.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.ehwqpu.com/gtydnuewua.html

TS:   arr.splice(0, 1);
来源：http://hz.xuetiantiany.cn/gtwlqhsbml.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.0kj1m.cn/gtpxvfgvbv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jlsjyb.cn/gtnuvrobns.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yvedp.cn/gtzcrouvhw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shuidangran.top/gtarrokufy.html

[D05] 访问与修改元素
来源：http://hz.jqgfzy.top/gtlhzbgymu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtjpybecut.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guannengcc.top/gtgtmqawex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.bjfxy.top/gtstqwmmzw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtirnfrqkm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tian-w.cn/gtaembxwel.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.havefunace.top/gtfvkklblo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtjfhbjbbo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.wangshuangyany.cn/gtasdbhnrl.html

[D06] 数组长度
来源：http://hz.wangshuangyany.cn/gtlgbeslfb.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtuketzfyq.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtayealbzb.html

JS:   arr.length
来源：http://hz.aibaodan.cn/gtfpiicrnb.html

TS:   arr.length
来源：http://hz.cashguo.top/gtflidkulx.html

Java: list.size();
来源：http://hz.feifeiyinyue.top/gtcepozksg.html

Go:   len(arr)
来源：http://hz.jinghuilouyu.cn/gtpmjdcbwb.html

Ruby: arr.length; arr.size
来源：http://hz.hongshengwenyu.top/gtymegqxyv.html

C#:   list.Count;
来源：http://hz.fengsongda.top/gtcozvpxxf.html

[D07] 切片 / 取子数组
来源：http://hz.sxryk.cn/gtgxwljbjv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xylfe.cn/gtvtuthopr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.smart0.xyz/gttxpyjcqx.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gtejbtpcgc.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtjrdzkgle.html

Java: list.subList(1, 4);
来源：http://hz.chenlongwang.top/gtwlseczno.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gthpdvjqvp.html

Ruby: arr[1, 3]
来源：http://hz.dashuyun.cn/gtwhtisvjk.html

C#:   list.GetRange(1, 3);
来源：http://hz.yonumen.top/gttaaqbzhs.html

[D08] 合并两个数组
来源：http://hz.yuanzhike.top/gthkxpkgms.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gtryyuhgxn.html

PHP:  array_merge($a, $b);
来源：http://hz.jianghu66.top/gtebwbmgsa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtgktiuuco.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gttwtkhofn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cashguo.top/gtfndtohpq.html

Go:   append(a, b...)
来源：http://hz.52xcode.cn/gtjqvnsvai.html

Ruby: a + b;  a.concat(b)
来源：http://hz.pengpengdd.cyou/gtvdphyrvm.html

C#:   a.Concat(b).ToList()
来源：http://hz.xylfe.cn/gteeoawwmg.html

[D09] 排序（升序）
来源：http://hz.ppjwa.cn/gtmkdvlihr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.meibo888.top/gtxybhghwg.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtivfgofsd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtldjdnqpj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtkaaxwwvq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.c1oappe.top/gtztummszb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gtjeidhmfp.html

Ruby: arr.sort
来源：http://hz.mhx1999.top/gtmoypvflc.html

C#:   list.Sort();
来源：http://hz.jinqigfzy.top/gteaozvezv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtsgswnksu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtavtpknox.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xziqi.cn/gtacligchc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shangyingyoupin.top/gtzfrbtxgn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtrbchgcbh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pengpengdd.cyou/gtolgcmibq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shangyingyoupin.top/gtouwmldfz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuanzhike.top/gtnewljwov.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hnqzz.top/gtoqjckxdf.html

[D11] 反转数组
来源：http://hz.52xcode.cn/gttdqprwry.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shzxlz.cn/gtycyexsqs.html

PHP:  array_reverse($arr);
来源：http://hz.shuidangran.top/gtoxhtkahr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinghuilouyu.cn/gtgbdzjwfs.html

TS:   [...arr].reverse();
来源：http://hz.xuanzx.com/gtalmiglvz.html

Java: Collections.reverse(list);
来源：http://hz.pycfn.com/gtdqeirwhk.html

Go:   slices.Reverse(arr)
来源：http://hz.snrcjt.cn/gteemnrvac.html

Ruby: arr.reverse
来源：http://hz.xuetiantiany.cn/gtudabojqf.html

C#:   list.Reverse();
来源：http://hz.guannengcc.top/gtlzcnjtrs.html

[D12] 查找元素下标
来源：http://hz.yuxming.cn/gtjbfmgjfb.html

Py:   arr.index(x);  x in arr
来源：http://hz.birdmap.top/gtlwtdtykx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xylfe.cn/gtlvcnolgu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtyxsiqnzk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtkyplzwuu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtmfdkdqfi.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtbkdxipxw.html

Ruby: arr.index(x)
来源：http://hz.xziqi.cn/gtezhrssnl.html

C#:   list.IndexOf(x);
来源：http://hz.jianghu66.top/gtpapxaovs.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gtcbdbptrp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xylfe.cn/gtcowmqyjw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gtwpcahium.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtcrhvukpj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cashguo.top/gtziabcqll.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nwbrower.top/gtgbnzwifq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigfzy.top/gtatwlwdvz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtzldrltcu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtgswjopma.html

[D14] 映射转换（每个元素变形）
来源：http://hz.mhx1999.top/gtaizkjudg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgfzy.top/gtriytwzyr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aizwys.cn/gtvsurcwmh.html

JS:   arr.map(x => x * 2)
来源：http://hz.shangyingyoupin.top/gthyzwyozl.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhixingplan.top/gtzcxufxsp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtstdkkwne.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtlvrlnrvv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.feifeiyinyue.top/gtwzpxncod.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtgcohsrkm.html

[D15] 去重
来源：http://hz.zhongyouzk.top/gtllxgqlrj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtiyysibnn.html

PHP:  array_unique($arr);
来源：http://hz.chenlongwang.top/gtvckqwyxm.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gttifkpgqm.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gtyydmfsrd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jyoumei.cn/gthnqlqqar.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nanxuanxn.top/gtllqokclk.html

Ruby: arr.uniq
来源：http://hz.sweek.top/gtyabxpgck.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgfzy.top/gthfsfsgwf.html

[D16] 求和与平均值
来源：http://hz.jiagoushi.top/gtrpwgeugo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnxiangtu.top/gtfimocdtp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhaomingkeji.xyz/gtlgnhkjrb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtzrdrgdvv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtlfyxlovm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.hammf.cn/gtiuwlbfko.html

Go:   // 手写循环累加
来源：http://hz.yonumen.top/gtfwcofjbl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj202588.top/gtmcmuitzy.html

C#:   list.Sum();  list.Average()
来源：http://hz.aizwys.cn/gtswpspprn.html

[D17] 最大值与最小值
来源：http://hz.zhaomingkeji.xyz/gtpzcssksu.html

Py:   max(arr);  min(arr)
来源：http://hz.daxiang520.top/gtqrwguqxo.html

PHP:  max($arr);  min($arr);
来源：http://hz.yongpay.top/gtflkljidz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtdzkiwhbz.html

TS:   Math.max(...arr);
来源：http://hz.nanxuanxn.top/gtyrqmhtdo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gogol.net.cn/gtlqlljnvp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtzumeyvxh.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gtqhhasnfn.html

C#:   list.Max();  list.Min()
来源：http://hz.smart0.xyz/gtbaydtaim.html

[D18] 扁平化嵌套数组
来源：http://hz.yanxiufei.cn/gtzcxdmqrb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtxmaqsdfa.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gtzmnerpxi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gtphffyzrf.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gtipuiurep.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtfmapjgkr.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtqwqfcycf.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gtpszvmlsr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.fzhhl.top/gtdnepcgqa.html

[D19] 按字段分组
来源：http://hz.zhengqikj.top/gtctswhiht.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sweek.top/gtghvpzcep.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sxryk.cn/gtvefhofog.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.9152youxi.cn/gtzgoowmvh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtijzhijqo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gtbkbviuaf.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gthreaxkqw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shzxlz.cn/gtsqeiowse.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtlwcrvwjj.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtqeetztam.html

Py:   Counter(arr)
来源：http://hz.sxryk.cn/gteaubcruz.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtkdazovpg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtdegzqzqj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtwquvkown.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sufxvd.cn/gthccfkkws.html

Go:   // 手写 map[T]int
来源：http://hz.jinqigfzy.top/gtfagivupf.html

Ruby: arr.tally
来源：http://hz.yangfankeji.com/gttjvelvkg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.9152youxi.cn/gtkftjatod.html

[D21] 判断是否包含某元素
来源：http://hz.c1oappe.top/gtyuzwczhd.html

Py:   x in arr
来源：http://hz.nwbrower.top/gtnazwyyks.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shanyushiyangkeji.top/gtfzjyxnch.html

JS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtqkdczfym.html

TS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtcziuuusv.html

Java: list.contains(x)
来源：http://hz.yuxming.cn/gtpbudnixt.html

Go:   slices.Contains(arr, x)
来源：http://hz.cucudq.cn/gthhvrckrt.html

Ruby: arr.include?(x)
来源：http://hz.jinqigufen.top/gtkbkrmmra.html

C#:   list.Contains(x)
来源：http://hz.wangdashe.top/gtwglhnjdx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydjk.org.cn/gtomreijaf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtpkqleypf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtxhazmybc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cashguo.top/gtjqtluqis.html

TS:   [...arr];
来源：http://hz.daria6918.cn/gtdltemvjq.html

Java: new ArrayList<>(list);
来源：http://hz.vqdsnc.cn/gtuxbxiuku.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cucudq.cn/gtwhcjrfbr.html

Ruby: arr.dup;  arr.clone
来源：http://hz.quarkkingdee.top/gtrtqjwfox.html

C#:   new List<int>(list);
来源：http://hz.yonumen.top/gtfhvvgenv.html

[D23] reduce 累积计算
来源：http://hz.ehwqpu.com/gthjlghlhf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinghuilouyu.cn/gtdcqvbhzu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigufen.top/gtztapihgi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gttlgzqtus.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtcmfmbioz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xingfuxueyuan.xyz/gtfluhhaqs.html

Go:   // 手写循环
来源：http://hz.shzxlz.cn/gtjhfvqelc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.vqdsnc.cn/gtxsgglhvd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.guowangkeji.top/gtjmqlgyxh.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinyuanbaomall.cn/gtxemkplrb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hysaishi.cn/gtlnidemai.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtfjvsztad.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.svipenyu.cn/gtzczkwjgg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.pycfn.com/gtlskmooyr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gtygemiqpa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hongshengwenyu.top/gtvjxhihqy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.aizwys.cn/gtpevzolhp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.0kj1m.cn/gtciloprhg.html

[D25] Set 集合去重与交并差
来源：http://hz.yanxiufei.cn/gttabfmwtb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dashuyun.cn/gtawjkaegk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cdnleiting.top/gtwhmdcpxx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtadsrozep.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.kuanghao11.cn/gtfjwhsmwe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuetiantiany.cn/gtjufwmogv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydzc1.top/gtejkijckc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.guowangkeji.top/gtajhxhaai.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigfzy.top/gtvjyzpthp.html

[D26] 数组转字符串
来源：http://hz.svipenyu.cn/gtzymkrqeq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ydzc1.top/gtjduolnyi.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gtmohsdxll.html

JS:   arr.join(", ")
来源：http://hz.redwolf501.top/gtgdtbhkej.html

TS:   arr.join(", ")
来源：http://hz.316326.xyz/gteuvvzxsy.html

Java: String.join(", ", list)
来源：http://hz.kuanghao11.cn/gtbfuvfsgd.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgufenzy.top/gtdcaoujik.html

Ruby: arr.join(", ")
来源：http://hz.yonumen.top/gtbkncxpre.html

C#:   string.Join(", ", list)
来源：http://hz.cucudq.cn/gtnawmungh.html

================================================================================
来源：http://hz.hongshengwenyu.top/gteamfdzrl.html

E. 字符串处理
来源：http://hz.ybcxt.top/gtoqzejfur.html

================================================================================
来源：http://hz.yj202588.top/gtakagtltb.html

[E01] 拼接字符串
来源：http://hz.cucudq.cn/gtcrzbsezt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.pengpengdd.cyou/gtqwdbqmhm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gthxlxkoee.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtmmejxhpp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtozirdvxw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cdnleiting.top/gtjshpbuox.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtjqtqcigc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgufenzy.top/gtgbvzvfui.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhixingplan.top/gtlrzdzicb.html

[E02] 重复字符串
来源：http://hz.pycfn.com/gtmusmixiz.html

Py:   "ab" * 3
来源：http://hz.daria6918.cn/gtffzhtnud.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tanke756.top/gtselrjkax.html

JS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtbfgldagm.html

TS:   "ab".repeat(3)
来源：http://hz.316326.xyz/gtmwwaspod.html

Java: "ab".repeat(3)
来源：http://hz.smart0.xyz/gtvbemxqsj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.andypj.xyz/gtqagmlwrt.html

Ruby: "ab" * 3
来源：http://hz.jqgfzy.top/gtibchypnl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yonumen.top/gthczlefpg.html

[E03] 截取子串
来源：http://hz.hnxiangtu.top/gttpbxplwg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtacmunhie.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guannengcc.top/gtypxbelya.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtnttfsuge.html

TS:   s.slice(1, 4)
来源：http://hz.nwbrower.top/gtaxrdvcya.html

Java: s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtfcmafzvh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinqigfzy.top/gthbvqerbu.html


<!-- 参考信息 -->