代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://hz.wangshuangyany.cn/gtwjcqngzd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhijiandao.cn/gtjgxcqifl.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigufen.top/gtxrcvwbag.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cashguo.top/gtykdvqbbc.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.quarkkingdee.top/gtdwsspdkv.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gthisnallg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.iojbl.cn/gtcfejzgcg.html

[C13] 类型声明 / 类型注解
来源：http://hz.316326.xyz/gtuqblqwwe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.haohaochexian.top/gthslkevhj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtsonurxol.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtbhcqlmnd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtkgtoqchq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.c1oappe.top/gtuhbigbuf.html

Go:   func add(a, b int) int
来源：http://hz.shangyingyoupin.top/gtpkbjzkbv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.chenzaomai.com/gtmlioranv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hywenlv.cn/gtnztkvktk.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtenesvwwc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.feifeiyinyue.top/gtorsvfzkw.html

PHP:  // 无泛型
来源：http://hz.redwolf501.top/gtqpumrixv.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtepnzuxbg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gaohongyu789.top/gtsyizrniw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.havefunace.top/gtdklmpsxn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gtktqdwtnx.html

Ruby: # 无泛型
来源：http://hz.jlsjyb.cn/gtihzxgeib.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sxryk.cn/gthmaiignm.html

[C15] 解构 / 展开参数
来源：http://hz.ppjwa.cn/gtjvdekjfz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtxnjmkcws.html

PHP:  [$a, $b] = $pair;
来源：http://hz.wangdashe.top/gteplqtumf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.ydjk.org.cn/gtmukhquao.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtammmcdvw.html

Java: // 无解构
来源：http://hz.zycfv.cn/gtptkzjoiz.html

Go:   // 无解构
来源：http://hz.xylfe.cn/gtckedgdei.html

Ruby: a, b = pair
来源：http://hz.ybcxt.top/gtudfbrpae.html

C#:   var (a, b) = pair;
来源：http://hz.hfpthk.cn/gtcvpluege.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtuarbllvd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tanke756.top/gterhcrdyf.html

PHP:  // 无重载
来源：http://hz.zhijiandao.cn/gttkmvtgcw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gttqnmylge.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtifserhvk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xuanzx.com/gtqodpxzrd.html

Go:   // 无重载：用不同函数名
来源：http://hz.xinyue.icu/gtfcrpaabb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sxryk.cn/gtbjqaqlhy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.daria6918.cn/gtyflsfqeu.html

================================================================================
来源：http://hz.yueranfly.top/gtjphmhwxm.html

D. 数组 / 列表 / 集合
来源：http://hz.mhx1999.top/gtglfedclt.html

================================================================================
来源：http://hz.nanxuanxn.top/gtihbvaxqn.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtiikkfkkz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.svipenyu.cn/gtivmddobj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ivvv.top/gtxebotewb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxuanxn.top/gtkhwezina.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.chenjidiqi.icu/gtnlammrni.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gthwhxsldy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xingfuxueyuan.xyz/gtsayabttd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pengpengdd.cyou/gtkhbmeuje.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.chenjidiqi.icu/gtvshxquar.html

[D02] 追加元素到末尾
来源：http://hz.xylfe.cn/gtxfmqwkut.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gaohongyu789.top/gtnpaurvhw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtniefznuy.html

JS:   arr.push(4);
来源：http://hz.jinqigufen.top/gtytylnyqg.html

TS:   arr.push(4);
来源：http://hz.ybcxt.top/gtrzbvwgis.html

Java: list.add(4);
来源：http://hz.tanke756.top/gtszvemujr.html

Go:   arr = append(arr, 4)
来源：http://hz.yueranfly.top/gtqbvaxyjx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hammf.cn/gtgolijyag.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gttewfgxag.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtbkdhugbh.html

Py:   arr.insert(0, 0)
来源：http://hz.cqqwz.cn/gtyvlskewc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtsfwqxibp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.316326.xyz/gtfmbsayyj.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yj20258888.top/gtdsvbwela.html

Java: list.add(0, 0);
来源：http://hz.gogol.net.cn/gtdoewfwgd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hongshengwenyu.top/gtmkthigqs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shzxlz.cn/gtnmdjcqpy.html

C#:   list.Insert(0, 0);
来源：http://hz.zdqjudy.top/gttjeskwsb.html

[D04] 删除元素
来源：http://hz.yuanzhike.top/gtllbrycsc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.bjfxy.top/gtfzlqiltj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.pycfn.com/gtlaqkevav.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtefgkeshd.html

TS:   arr.splice(0, 1);
来源：http://hz.tianlin.xyz/gtsqlsmmuq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yueranfly.top/gtwkzvvjnk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.dianchejie.cn/gtxtdjlrtk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yangfankeji.com/gtjpgdxsze.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zdqjudy.top/gtblwiqupl.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtdqlethtv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtjmanebdr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.quarkkingdee.top/gtiicilnsv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuxming.cn/gtzbmnplmk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.guannengcc.top/gtwvsohwom.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cashguo.top/gtvkmvofdi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gtwmxtygff.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtvvbgyijy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgufenzy.top/gtyxtwjoup.html

[D06] 数组长度
来源：http://hz.ehwqpu.com/gtobetgwzr.html

Py:   len(arr)
来源：http://hz.pengpengdd.cyou/gttvbjyozr.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtgrzridwb.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtfekqsnpx.html

TS:   arr.length
来源：http://hz.tianlin.xyz/gttymnjobq.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtpzxcqwvr.html

Go:   len(arr)
来源：http://hz.wangshuangyany.cn/gtahhgjxqs.html

Ruby: arr.length; arr.size
来源：http://hz.sxryk.cn/gtgwlvkqdd.html

C#:   list.Count;
来源：http://hz.zhongyouzk.top/gtqazjilxd.html

[D07] 切片 / 取子数组
来源：http://hz.iojbl.cn/gtnpbzstlb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.0kj1m.cn/gtawxfbhnc.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jyoumei.cn/gtvqzpdugj.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gtfckcajla.html

TS:   arr.slice(1, 4);
来源：http://hz.zhoulong.xyz/gtgchvdqqa.html

Java: list.subList(1, 4);
来源：http://hz.zhongyouzk.top/gtzhceifhs.html

Go:   arr[1:4]
来源：http://hz.yueranfly.top/gtllaqzive.html

Ruby: arr[1, 3]
来源：http://hz.hammf.cn/gtvwvatvfe.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxuanxn.top/gtbrkxdshy.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gtsjecjmtk.html

Py:   a + b;  a.extend(b)
来源：http://hz.mhx1999.top/gtfhonxsgk.html

PHP:  array_merge($a, $b);
来源：http://hz.wangdashe.top/gtuznefkje.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hywenlv.cn/gtsdphkeeh.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtqblpjpya.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shuidangran.top/gtbbqncwwy.html

Go:   append(a, b...)
来源：http://hz.tanke756.top/gtgmlzlgap.html

Ruby: a + b;  a.concat(b)
来源：http://hz.wangdashe.top/gtnaijxjsj.html

C#:   a.Concat(b).ToList()
来源：http://hz.yonumen.top/gtqgnmcmwh.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtpqrzqbog.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtzevwfckw.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtxubgtexi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tanke756.top/gtxstnvkgu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ivvv.top/gtxlzckjjd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgufenzy.top/gtofcrssgz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cqqwz.cn/gtwuqtypmh.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtkohpjpkz.html

C#:   list.Sort();
来源：http://hz.ywan-chungtsiang.top/gtkvaultmj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.haohaochexian.top/gtangqutxo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.tanke756.top/gtpvolcnxv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daxiang520.top/gtubtzzuds.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.9152youxi.cn/gtizmoerah.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtclzewtrj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.aibaodan.cn/gtjecqgzpn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hysaishi.cn/gtsqmybwuq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ywan-chungtsiang.top/gthfgeioqj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nwbrower.top/gtztokglys.html

[D11] 反转数组
来源：http://hz.yangfankeji.com/gtszumrxys.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gaohongyu789.top/gtulveijis.html

PHP:  array_reverse($arr);
来源：http://hz.gogol.net.cn/gtnhnssyag.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtnbkdzjcz.html

TS:   [...arr].reverse();
来源：http://hz.feifeiyinyue.top/gtbsizdpzc.html

Java: Collections.reverse(list);
来源：http://hz.cqqwz.cn/gtvwurxckf.html

Go:   slices.Reverse(arr)
来源：http://hz.ydjk.org.cn/gtetedqkiv.html

Ruby: arr.reverse
来源：http://hz.zhongyouzk.top/gtkdypxyqe.html

C#:   list.Reverse();
来源：http://hz.yuxming.cn/gtjcrnicrs.html

[D12] 查找元素下标
来源：http://hz.xuanzx.com/gtmnjcdlxv.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gtgynfwvjw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.smart0.xyz/gtdlrxdpsr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtsjajucrc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtycpkdxgu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ybcxt.top/gturrnzskj.html

Go:   slices.Index(arr, x)
来源：http://hz.jyoumei.cn/gtmkpmigbu.html

Ruby: arr.index(x)
来源：http://hz.hnqzz.top/gtjkowsmpj.html

C#:   list.IndexOf(x);
来源：http://hz.gzhubu.top/gthdufuzpc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xziqi.cn/gtmuzohcnz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shzxlz.cn/gtqudqwbzf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.vqdsnc.cn/gtddjapeyz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtuskmltou.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtwaxcqbid.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gthhbdipso.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtuhorvbfz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgufenzy.top/gtxumtwljv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fzhhl.top/gtosuepzfw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nanxuanxn.top/gtjvgsbttu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.birdmap.top/gtunbclauv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gzhubu.top/gteyrvjojl.html

JS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtibcvvxrq.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtbfhxhpje.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigufen.top/gtuqdnrdzc.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtxblkcdvi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.fzhhl.top/gtahotcpzb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jyoumei.cn/gtdhkswcgk.html

[D15] 去重
来源：http://hz.bjfxy.top/gtsiwoznin.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hongshengwenyu.top/gtrqnebpkf.html

PHP:  array_unique($arr);
来源：http://hz.quarkkingdee.top/gtthairofn.html

JS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtfsiuntnq.html

TS:   [...new Set(arr)]
来源：http://hz.xylfe.cn/gtqttwvvit.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yanxiufei.cn/gthzfedqxh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.vqdsnc.cn/gtcchytsmr.html

Ruby: arr.uniq
来源：http://hz.sxryk.cn/gtokgtsmpz.html

C#:   list.Distinct().ToList()
来源：http://hz.yonumen.top/gtahviflhb.html

[D16] 求和与平均值
来源：http://hz.tianlin.xyz/gtlxfnzfvf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.bjfxy.top/gtbijaxulx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.52xcode.cn/gtnlcppbpi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtigtygyqh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtwblxpwbq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aizwys.cn/gtjtstotsv.html

Go:   // 手写循环累加
来源：http://hz.zhoulong.xyz/gtydogfsau.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hfpthk.cn/gticffvftp.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtixbfterp.html

[D17] 最大值与最小值
来源：http://hz.hnqzz.top/gtbmodzcur.html

Py:   max(arr);  min(arr)
来源：http://hz.gogol.net.cn/gthamhltzx.html

PHP:  max($arr);  min($arr);
来源：http://hz.feifeiyinyue.top/gtdlbhquhp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangdashe.top/gtrlaejuor.html

TS:   Math.max(...arr);
来源：http://hz.pycfn.com/gtomxfcnyd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ywan-chungtsiang.top/gtlbqfaxfd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.shzxlz.cn/gtndrvkuwi.html

Ruby: arr.max;  arr.min
来源：http://hz.jinghuilouyu.cn/gtuuunlufu.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtctfaeyjo.html

[D18] 扁平化嵌套数组
来源：http://hz.316326.xyz/gttopdpdxi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ywan-chungtsiang.top/gtdlvvmage.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtheqeupgq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gzhubu.top/gtdqemnmkx.html

TS:   nested.flat();
来源：http://hz.52xcode.cn/gtiskuocet.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangtech.top/gteycfahab.html

Go:   // 手写双层循环
来源：http://hz.ehwqpu.com/gtzbgghwvj.html

Ruby: nested.flatten
来源：http://hz.jyoumei.cn/gtyipmmxmz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenlongwang.top/gtmehmgehr.html

[D19] 按字段分组
来源：http://hz.xuanzx.com/gtrmtioxit.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xylfe.cn/gtpvtlargz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtunpirrha.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hammf.cn/gtsdseabis.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gtxgqofoqu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.aizwys.cn/gtcngdppjf.html

Go:   // 手写 map[string][]T
来源：http://hz.dianchejie.cn/gtwcrzgwln.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hfpthk.cn/gtzioxbkrl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtgyfxpplx.html

[D20] 统计每个元素出现次数
来源：http://hz.gzhubu.top/gtopefojti.html

Py:   Counter(arr)
来源：http://hz.aizwys.cn/gtzomgsfeo.html

PHP:  array_count_values($arr);
来源：http://hz.sysykeji.top/gtobjhivha.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtskfmmbfc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.aibaodan.cn/gtbjuyjpdw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xingfuxueyuan.xyz/gtldegbine.html

Go:   // 手写 map[T]int
来源：http://hz.ivvv.top/gtxjjvkruu.html

Ruby: arr.tally
来源：http://hz.wangshuangyany.cn/gtjxjymkcn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zycfv.cn/gtvqiaioam.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtavqsmqab.html

Py:   x in arr
来源：http://hz.vqdsnc.cn/gtfixbvxbn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gtdjdnfyfz.html

JS:   arr.includes(x)
来源：http://hz.hnqzz.top/gtdlehlgct.html

TS:   arr.includes(x)
来源：http://hz.yj202588.top/gtdlyksdrw.html

Java: list.contains(x)
来源：http://hz.smart0.xyz/gtgdalsocb.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtenzyshdt.html

Ruby: arr.include?(x)
来源：http://hz.wangshuangyany.cn/gtnnhbduaj.html

C#:   list.Contains(x)
来源：http://hz.dianchejie.cn/gtslashjqj.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenjidiqi.icu/gtwwdoygnp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tianlin.xyz/gtaaswmpln.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gtqzqtfgiz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.pengpengdd.cyou/gtfuvkvmkp.html

TS:   [...arr];
来源：http://hz.aizwys.cn/gtmhgqqcge.html

Java: new ArrayList<>(list);
来源：http://hz.xylfe.cn/gtdypdymgw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuanzhike.top/gtvsjuzirl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtqpcvjifz.html

C#:   new List<int>(list);
来源：http://hz.yj202588.top/gtmntmkeku.html

[D23] reduce 累积计算
来源：http://hz.52xcode.cn/gtpafyeapy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yangfankeji.com/gtapozncvd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jiagoushi.top/gtbfmrcmza.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gotoacloud.top/gtpcvynpds.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtfaemedsb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yvedp.cn/gtbwrqxhbw.html

Go:   // 手写循环
来源：http://hz.nanxinkj.top/gtmcmaiehb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shuidangran.top/gtgpztjtgj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtpmngcxod.html

[D24] 字典 / Map 基本操作
来源：http://hz.hywenlv.cn/gtalrcbwwv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hfpthk.cn/gtvgbaraiu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gtpjorwezs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ivvv.top/gthrfacaip.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydjk.org.cn/gtbcbfzdil.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xziqi.cn/gtmqiudfrz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtyxowvbnb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.haohaochexian.top/gtnswsslij.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinyuanbaomall.cn/gtiebifbmq.html

[D25] Set 集合去重与交并差
来源：http://hz.yangfankeji.com/gtpewldnno.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtjrlzxaqg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtiiohihwp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj20258.top/gtbihwcegs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hnqzz.top/gtfrhbjenr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shangyingyoupin.top/gtjbxfadiz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tanke756.top/gtbxshvfve.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tanke756.top/gtlcvjydai.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yongpay.top/gtxotomqtt.html

[D26] 数组转字符串
来源：http://hz.yonumen.top/gtptxravzz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gtieknxqyd.html

PHP:  implode(", ", $arr);
来源：http://hz.cqqwz.cn/gtezgzykax.html

JS:   arr.join(", ")
来源：http://hz.yonumen.top/gtatixdfza.html

TS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtyqjbpbeb.html

Java: String.join(", ", list)
来源：http://hz.yanxiufei.cn/gtxzfhfwmp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hammf.cn/gtlpilelnr.html

Ruby: arr.join(", ")
来源：http://hz.gaohongyu789.top/gteyqoevfn.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gtgyowglle.html

================================================================================
来源：http://hz.xuanzx.com/gtlctcbfpu.html

E. 字符串处理
来源：http://hz.hongshengwenyu.top/gtllsggpro.html

================================================================================
来源：http://hz.gzhubu.top/gtysjudjyh.html

[E01] 拼接字符串
来源：http://hz.sxryk.cn/gtmslfyobt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gogol.net.cn/gtqyyejibs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.xinyue.icu/gtulgkzxwk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuxming.cn/gthhpgverc.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtbvludunz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.chenjidiqi.icu/gtxkmfcbjf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.andypj.xyz/gtabbbslhp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtnzppdpeb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gtszvnqaof.html

[E02] 重复字符串
来源：http://hz.ivvv.top/gtwcacikyi.html

Py:   "ab" * 3
来源：http://hz.yj20258888.top/gtznzxkrly.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ydjk.org.cn/gtuoxtcjng.html

JS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gtbnrdnhnz.html

TS:   "ab".repeat(3)
来源：http://hz.pycfn.com/gtxykkxszl.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gthqhvoiyj.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ywan-chungtsiang.top/gtygxuzgxo.html

Ruby: "ab" * 3
来源：http://hz.jinqigfzy.top/gtiiofbkfd.html


<!-- 参考信息 -->