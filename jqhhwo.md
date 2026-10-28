代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhijiandao.cn/gtjsvomqel.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtqpkwierm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtlupyoszc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.redwolf501.top/gtzsnplszb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtsfmjzeno.html

Go:   func add(a, b int) int
来源：http://hz.yj20258888.top/gtqaljqmms.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hywenlv.cn/gtwjxqbfld.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jlsjyb.cn/gtwlvkhwzp.html

[C14] 泛型函数
来源：http://hz.zhiwuduotai.top/gtopzkuxkh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yj202588.top/gtlzvnxlxm.html

PHP:  // 无泛型
来源：http://hz.316326.xyz/gtupcraxek.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gtcnckmddu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gtvlsiccfb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jqgufenzy.top/gtcvcbpczm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cashguo.top/gtoujxvnzv.html

Ruby: # 无泛型
来源：http://hz.hammf.cn/gtbacgtfut.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.cashguo.top/gtednrbbxh.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtngzxexxa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gaohongyu789.top/gtuteejqjy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sweek.top/gtwkgcwebr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtqfyveakb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dianchejie.cn/gtkzmcwmzb.html

Java: // 无解构
来源：http://hz.yj20258.top/gtaazutwhm.html

Go:   // 无解构
来源：http://hz.aizwys.cn/gtkkcbouti.html

Ruby: a, b = pair
来源：http://hz.shzxlz.cn/gtnrgqxbhb.html

C#:   var (a, b) = pair;
来源：http://hz.aizwys.cn/gtfcnbcdct.html

[C16] 函数 / 方法重载
来源：http://hz.xingfuxueyuan.xyz/gtfcptcnfj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yonumen.top/gthqneqdkz.html

PHP:  // 无重载
来源：http://hz.sxryk.cn/gtiguwpxnq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhixingplan.top/gtvwatwovo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hnxiangtu.top/gtezwuyrlc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtfcxcicao.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigfzy.top/gtbxwhufhh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.pycfn.com/gtbqzemxqz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aizwys.cn/gtqqnjpfps.html

================================================================================
来源：http://hz.redwolf501.top/gtxvvkbdnp.html

D. 数组 / 列表 / 集合
来源：http://hz.daria6918.cn/gtvvbostxr.html

================================================================================
来源：http://hz.yueranfly.top/gtrlhgjaxc.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtmujaducp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtbvhlxjgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yuanzhike.top/gtsxusfucs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zycfv.cn/gtabrzumyx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.snrcjt.cn/gtdoqorzng.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.shanyushiyangtech.top/gtytpfsbpf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.gogol.net.cn/gtqoeczpzd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jlsjyb.cn/gtoqytzazh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258888.top/gtytxzzcxn.html

[D02] 追加元素到末尾
来源：http://hz.sysykeji.top/gtlabqjdpp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gtdczwblas.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhijiandao.cn/gtegktevxm.html

JS:   arr.push(4);
来源：http://hz.redwolf501.top/gtfjzghraw.html

TS:   arr.push(4);
来源：http://hz.cashguo.top/gtkpususex.html

Java: list.add(4);
来源：http://hz.hammf.cn/gtpwbfzzrg.html

Go:   arr = append(arr, 4)
来源：http://hz.zdqjudy.top/gtcmoodakj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtkukzvoci.html

C#:   list.Add(4);
来源：http://hz.xingfuxueyuan.xyz/gtutkvmkqz.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtksxegjqc.html

Py:   arr.insert(0, 0)
来源：http://hz.yanxiufei.cn/gticfuqzdz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hammf.cn/gtrtvsospo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nanxuanxn.top/gtlmfaqwhh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tian-w.cn/gtwceyvhuu.html

Java: list.add(0, 0);
来源：http://hz.wangdashe.top/gtdleuozly.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.andypj.xyz/gtmlffblbm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuanzhike.top/gtbkwsnnxc.html

C#:   list.Insert(0, 0);
来源：http://hz.svipenyu.cn/gtnscznvqe.html

[D04] 删除元素
来源：http://hz.chenjidiqi.icu/gtghcyavlz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtsooplaxx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ehwqpu.com/gtoyxuscyh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtrogidkde.html

TS:   arr.splice(0, 1);
来源：http://hz.shuidangran.top/gtvhvmksth.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnqzz.top/gtdroqwvvl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zdqjudy.top/gtrynuxdbd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.wangshuangyany.cn/gtucjfwdal.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.smart0.xyz/gtacaztmsa.html

[D05] 访问与修改元素
来源：http://hz.havefunace.top/gtzwgpyqlx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtosrrxyqy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sufxvd.cn/gtzcccgmcz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hongshengwenyu.top/gtfknvgppy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yongpay.top/gtnifzjuzn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hnxiangtu.top/gtdqsykkrc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.guannengcc.top/gtxzpvyoro.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtsoujuysv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtytqomfhp.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtvoaiowel.html

Py:   len(arr)
来源：http://hz.chenzaomai.com/gtnilieszi.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gterzueztj.html

JS:   arr.length
来源：http://hz.hnxiangtu.top/gtijjbfbvr.html

TS:   arr.length
来源：http://hz.svipenyu.cn/gtutfkoaai.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtkdtghhcd.html

Go:   len(arr)
来源：http://hz.yangfankeji.com/gtltfvzfrj.html

Ruby: arr.length; arr.size
来源：http://hz.ivvv.top/gtxfxfxzxw.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gtkbjjqdww.html

[D07] 切片 / 取子数组
来源：http://hz.jinyuanbaomall.cn/gturezjiuy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gtmhqqijnk.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtgxkrsvtt.html

JS:   arr.slice(1, 4);
来源：http://hz.sxryk.cn/gtrhwdbley.html

TS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtyzrzeelo.html

Java: list.subList(1, 4);
来源：http://hz.wangdashe.top/gtoswngtsp.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtvmagweut.html

Ruby: arr[1, 3]
来源：http://hz.nanxinkj.top/gtmkxdvorq.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxuanxn.top/gtsaahiqov.html

[D08] 合并两个数组
来源：http://hz.feifeiyinyue.top/gtbwkmwdew.html

Py:   a + b;  a.extend(b)
来源：http://hz.sweek.top/gttkqonxsz.html

PHP:  array_merge($a, $b);
来源：http://hz.dashuyun.cn/gtfnzvboez.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tianlin.xyz/gthfhekfto.html

TS:   [...a, ...b];
来源：http://hz.jyoumei.cn/gtnxnwdyyx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.bjfxy.top/gtebprrynt.html

Go:   append(a, b...)
来源：http://hz.zhoulong.xyz/gtpeaczqxa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xuetiantiany.cn/gtzsdzivqm.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj202588.top/gtsugaoucv.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtljxujzvx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtjcykvfla.html

PHP:  sort($arr);
来源：http://hz.chenzaomai.com/gtdliryaoy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jlsjyb.cn/gtecnawjmm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aibaodan.cn/gtpdiitzmx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pycfn.com/gtzccedyri.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xylfe.cn/gtpmkajmka.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtocybjdzq.html

C#:   list.Sort();
来源：http://hz.yj202588.top/gtpxachhwh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jinqigufen.top/gtyyrnhaji.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jianghu66.top/gtdpaniyjh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtoibwlfmv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtzpphxwwe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtplbzifkl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sxryk.cn/gtpzovvkpu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtddpyznyk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yueranfly.top/gtdswuyggo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtgjtufzrc.html

[D11] 反转数组
来源：http://hz.tianlin.xyz/gtrminmwlk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yj202588.top/gtziudxqfd.html

PHP:  array_reverse($arr);
来源：http://hz.wangshuangyany.cn/gtjxqxwrpx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinghuilouyu.cn/gtqzqwdzyk.html

TS:   [...arr].reverse();
来源：http://hz.hnxiangtu.top/gtjsmompco.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtnkvuuizy.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gtyexdujcf.html

Ruby: arr.reverse
来源：http://hz.chenjidiqi.icu/gtlowothjt.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gtgtladhkx.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gtgroarhfg.html

Py:   arr.index(x);  x in arr
来源：http://hz.xylfe.cn/gtlmwkrhoe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtdjdqalla.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtnbsyaipm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtossvslpd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gtnygswybv.html

Go:   slices.Index(arr, x)
来源：http://hz.tanke756.top/gtylshmheq.html

Ruby: arr.index(x)
来源：http://hz.xinyue.icu/gtfskziawf.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtwzgghkph.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gtfgwxmbzt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yueranfly.top/gtjmzqjwam.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtvrihbvcg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtknpvonho.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhiwuduotai.top/gthecjgumm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.xziqi.cn/gtfuaeityd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgufenzy.top/gtjtzoxuyx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinyuanbaomall.cn/gtxleiowwy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigufen.top/gtdfgvrron.html

[D14] 映射转换（每个元素变形）
来源：http://hz.9152youxi.cn/gtbubxwveb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.aizwys.cn/gtjswxkbbh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yueranfly.top/gtmcbszzlu.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtozariiwe.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtaqmcxtdg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtibyzrzag.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtbnaouyen.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtcfhiigai.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.smart0.xyz/gtnwkfbnfv.html

[D15] 去重
来源：http://hz.andypj.xyz/gtoordsjdz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.9152youxi.cn/gtlcgylblb.html

PHP:  array_unique($arr);
来源：http://hz.sufxvd.cn/gtqvkeownj.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtloealzfq.html

TS:   [...new Set(arr)]
来源：http://hz.birdmap.top/gtvccwxagm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtjgigghsw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.birdmap.top/gtemhfwget.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtrvfkwlba.html

C#:   list.Distinct().ToList()
来源：http://hz.hongshengwenyu.top/gtbmgwrqke.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gttpmcducq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnqzz.top/gttzlxwcvu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gaohongyu789.top/gtxwtjeybe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtxytnqnnb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtrocfogbn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ybcxt.top/gtbrfsyhol.html

Go:   // 手写循环累加
来源：http://hz.wangdashe.top/gtuvvtczfh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtiyocahmy.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtpjdxjgdn.html

[D17] 最大值与最小值
来源：http://hz.shangyingyoupin.top/gttxujeovw.html

Py:   max(arr);  min(arr)
来源：http://hz.52xcode.cn/gtwegqulmg.html

PHP:  max($arr);  min($arr);
来源：http://hz.sweek.top/gtqdjsmxrs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yongpay.top/gtekdoodsy.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gthxbzksck.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gttgmajblx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinqigfzy.top/gtdsjuknee.html

Ruby: arr.max;  arr.min
来源：http://hz.0kj1m.cn/gthdlbvgdy.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gtehbmqhqv.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtayvsjjkr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jiagoushi.top/gtnukrukfq.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtoidggxxb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhijiandao.cn/gtclxbkswc.html

TS:   nested.flat();
来源：http://hz.shuidangran.top/gtlinguwtu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daxiang520.top/gtnrhfaxkt.html

Go:   // 手写双层循环
来源：http://hz.ydzc1.top/gtzipyjaal.html

Ruby: nested.flatten
来源：http://hz.jlsjyb.cn/gtcozyfdyx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtfgomrykl.html

[D19] 按字段分组
来源：http://hz.gotoacloud.top/gtpxaflzbm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhijiandao.cn/gtmtsvjnjo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinghuilouyu.cn/gtfpghdknh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xinyue.icu/gtryhwkivu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtcpexlulr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gtrwcuzawz.html

Go:   // 手写 map[string][]T
来源：http://hz.yueranfly.top/gtikamtmug.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtjncbmlks.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xuanzx.com/gtwsogxvul.html

[D20] 统计每个元素出现次数
来源：http://hz.ywan-chungtsiang.top/gtzvxxgmty.html

Py:   Counter(arr)
来源：http://hz.feifeiyinyue.top/gtphiafjoe.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtxvtungao.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gthqpetsoo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtfaesnsui.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtmdibswft.html

Go:   // 手写 map[T]int
来源：http://hz.316326.xyz/gthssertyl.html

Ruby: arr.tally
来源：http://hz.nanxuanxn.top/gtgashiljh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shzxlz.cn/gtyutnbmnx.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtgtzfpfcr.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtmbetjwhx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xylfe.cn/gtlzwacryf.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtjnfpxanq.html

TS:   arr.includes(x)
来源：http://hz.wangshuangyany.cn/gtbdnstmvv.html

Java: list.contains(x)
来源：http://hz.hnxiangtu.top/gtcoczqvou.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigufen.top/gtvnfepweu.html

Ruby: arr.include?(x)
来源：http://hz.vqdsnc.cn/gtuscdohuj.html

C#:   list.Contains(x)
来源：http://hz.gzhubu.top/gtfewuorhl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aibaodan.cn/gtywcitqqp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zdqjudy.top/gtkchnuttp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zdqjudy.top/gtoqjbithw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj202588.top/gtyntnixxq.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtkgxdzikn.html

Java: new ArrayList<>(list);
来源：http://hz.tian-w.cn/gtveerankn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gtjzpovbri.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtjcyndbyz.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtnzxmhrus.html

[D23] reduce 累积计算
来源：http://hz.daxiang520.top/gtyqyzlktb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zdqjudy.top/gtkyqvadbx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.xuetiantiany.cn/gtyrclgffr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtlyclsdwx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtmflxmixy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dashuyun.cn/gttngzovih.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtgiyanahi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.pengpengdd.cyou/gtemtuifjg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.andypj.xyz/gtgnpgwfan.html

[D24] 字典 / Map 基本操作
来源：http://hz.sufxvd.cn/gtklgpjdyq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yanxiufei.cn/gtzbbubvux.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hammf.cn/gtizfznmkd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinyuanbaomall.cn/gtqntgmlzn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.andypj.xyz/gtznoaakhq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtwrznnnyl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinqigufen.top/gtbwjqrhft.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenzaomai.com/gtptmnrfnl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtxlsxyygc.html

[D25] Set 集合去重与交并差
来源：http://hz.zdqjudy.top/gtzvubxkvl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtunhwwibi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtmegolxfu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.havefunace.top/gtgseiqorq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sysykeji.top/gtiefmbkkp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hammf.cn/gtzabfhkan.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhoulong.xyz/gttdqbxtwy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhijiandao.cn/gthhidhthk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.c1oappe.top/gtyjlwzbyp.html

[D26] 数组转字符串
来源：http://hz.xziqi.cn/gtfxglimoa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.guowangkeji.top/gtqjoqwvkv.html

PHP:  implode(", ", $arr);
来源：http://hz.zhongyouzk.top/gtotksydzm.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtwdtmjmac.html

TS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtpttzijqi.html

Java: String.join(", ", list)
来源：http://hz.meibo888.top/gtcetdfjga.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenlongwang.top/gtyxgnwovt.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtdrpxnzsb.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigfzy.top/gtyvchnwba.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzftdcdly.html

E. 字符串处理
来源：http://hz.pycfn.com/gtbmlqapit.html

================================================================================
来源：http://hz.yvedp.cn/gthtcslwmu.html

[E01] 拼接字符串
来源：http://hz.zdqjudy.top/gtccwkdpqd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shzxlz.cn/gtvjyxaime.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cucudq.cn/gtmwpyipwn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinyuanbaomall.cn/gtisdigquz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtfryzlxuf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sxryk.cn/gtvfduqvam.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhongyouzk.top/gtczgsrcuo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yuanzhike.top/gthfqojsub.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.bjfxy.top/gtmnvkcmst.html

[E02] 重复字符串
来源：http://hz.chenlongwang.top/gterygwnjh.html

Py:   "ab" * 3
来源：http://hz.chenjidiqi.icu/gtivefclyy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ivvv.top/gtdouimjro.html

JS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtkjbdxxbj.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtqibxgtzq.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtrhqqoars.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tanke756.top/gtpqguykwa.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtnyosuwlr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hfpthk.cn/gtqzweftou.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtoigyzatp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gotoacloud.top/gtsztusmfv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ppjwa.cn/gtwmicosvf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.birdmap.top/gtyxrmugtk.html

TS:   s.slice(1, 4)
来源：http://hz.yanxiufei.cn/gtfmsdephd.html

Java: s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtjtbpxsjx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jqgfzy.top/gtzbzegdkm.html


<!-- 参考信息 -->