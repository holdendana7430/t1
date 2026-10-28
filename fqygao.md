代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhiwuduotai.top/gtqdgzfzls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtwifsmtmq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jinyuanbaomall.cn/gtqrirhiky.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtxesuooru.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtzytvcjkm.html

Go:   func add(a, b int) int
来源：http://hz.iojbl.cn/gtjvjeqfrn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hfpthk.cn/gtrgsxqsix.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sxryk.cn/gteftdgkso.html

[C14] 泛型函数
来源：http://hz.daria6918.cn/gtvoabzwup.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtgzbqtimo.html

PHP:  // 无泛型
来源：http://hz.feifeiyinyue.top/gtmawkebba.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtnhbentcw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gtplcvqffw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtmusicgjr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hnqzz.top/gtbosxpxjb.html

Ruby: # 无泛型
来源：http://hz.tian-w.cn/gtupdmfcmp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daria6918.cn/gtprvvlzoo.html

[C15] 解构 / 展开参数
来源：http://hz.hysaishi.cn/gtebyfxmcp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ppjwa.cn/gtvfzowwwv.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cashguo.top/gtgbkjlbva.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtxeksgdsl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jlsjyb.cn/gtpaplilxr.html

Java: // 无解构
来源：http://hz.jqgfzy.top/gtzeasqagm.html

Go:   // 无解构
来源：http://hz.sysykeji.top/gtxjzloeyd.html

Ruby: a, b = pair
来源：http://hz.feifeiyinyue.top/gtdmqciotr.html

C#:   var (a, b) = pair;
来源：http://hz.quarkkingdee.top/gtkezmcwif.html

[C16] 函数 / 方法重载
来源：http://hz.yongpay.top/gthqwpyfqd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.52xcode.cn/gtgzxnnish.html

PHP:  // 无重载
来源：http://hz.9152youxi.cn/gtmbrxwoqr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.dashuyun.cn/gthymtpxhm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.guowangkeji.top/gtbyxhxrev.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xingfuxueyuan.xyz/gtmibjhcvm.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtzvmmwntw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xingfuxueyuan.xyz/gtpetimrsv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangshuangyany.cn/gtbyyriihv.html

================================================================================
来源：http://hz.tian-w.cn/gtzptwnuho.html

D. 数组 / 列表 / 集合
来源：http://hz.snrcjt.cn/gtklofvvvg.html

================================================================================
来源：http://hz.hfpthk.cn/gthvjwrftm.html

[D01] 创建数组 / 列表
来源：http://hz.ehwqpu.com/gtfmzveycn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cucudq.cn/gthmetgxhz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangdashe.top/gtyvxcbppe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gtxgdzrtzg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guannengcc.top/gtshuvthbw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.feifeiyinyue.top/gtzqlkmopp.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.guannengcc.top/gtpdfxxoph.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gtkrqexvxt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj20258.top/gtowyagptb.html

[D02] 追加元素到末尾
来源：http://hz.dianchejie.cn/gtvjpoxpkz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ivvv.top/gtbjdexxmj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gthfpqfasf.html

JS:   arr.push(4);
来源：http://hz.bjfxy.top/gtgvrhbfym.html

TS:   arr.push(4);
来源：http://hz.fzhhl.top/gtpbdgmkpy.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtpgiciybb.html

Go:   arr = append(arr, 4)
来源：http://hz.dashuyun.cn/gtjwtjguxq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhengqikj.top/gtibvqvwha.html

C#:   list.Add(4);
来源：http://hz.hnxiangtu.top/gtfbtodjum.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangtech.top/gtrqndtagp.html

Py:   arr.insert(0, 0)
来源：http://hz.sufxvd.cn/gtvqwflwih.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuxming.cn/gtldbkxupa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.iojbl.cn/gtpddcpupr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.daria6918.cn/gtgtbpqnnl.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtqtcfxels.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gtlcblcvub.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.daxiang520.top/gtlxtenojf.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtjtcsnqeo.html

[D04] 删除元素
来源：http://hz.cdnleiting.top/gtdgianwni.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenlongwang.top/gtlcvbkgct.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhoulong.xyz/gtktpmrpqn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.9152youxi.cn/gtmnvrdzlw.html

TS:   arr.splice(0, 1);
来源：http://hz.nanxinkj.top/gtgfokradm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gogol.net.cn/gtzkdebgsu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtmhrtulfl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sweek.top/gtkkjqlypg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.316326.xyz/gthbptatah.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gttatvliwl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gtrptxfxxg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shzxlz.cn/gtmhitnxio.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fzhhl.top/gtxbxpwwsg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xinyue.icu/gtqnnattfs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yonumen.top/gthtbyvoce.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gttfhzlifz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gtzurquubp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.nanxuanxn.top/gthmbsttng.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gtraknxpld.html

Py:   len(arr)
来源：http://hz.zhoulong.xyz/gtbvdhtsca.html

PHP:  count($arr);
来源：http://hz.zhengqikj.top/gtezbxvtwf.html

JS:   arr.length
来源：http://hz.yuxming.cn/gtgfjhaaiu.html

TS:   arr.length
来源：http://hz.yj20258.top/gtreggscwq.html

Java: list.size();
来源：http://hz.jianghu66.top/gtfuzlkpvg.html

Go:   len(arr)
来源：http://hz.zhiwuduotai.top/gtprjfvsxc.html

Ruby: arr.length; arr.size
来源：http://hz.meibo888.top/gtclmevbtr.html

C#:   list.Count;
来源：http://hz.yj20258888.top/gtfevhqolt.html

[D07] 切片 / 取子数组
来源：http://hz.jqgufenzy.top/gtxdvhxkpt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtsihynbqv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shzxlz.cn/gtbppeisvs.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtwokaluoh.html

TS:   arr.slice(1, 4);
来源：http://hz.c1oappe.top/gtjcxvzrhy.html

Java: list.subList(1, 4);
来源：http://hz.mhx1999.top/gtpokjzekr.html

Go:   arr[1:4]
来源：http://hz.zhiwuduotai.top/gtylhcngwg.html

Ruby: arr[1, 3]
来源：http://hz.birdmap.top/gtarfqiiyc.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangdashe.top/gtjzikgoqy.html

[D08] 合并两个数组
来源：http://hz.nanxinkj.top/gtxcvpkapn.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnxiangtu.top/gtbfrargbn.html

PHP:  array_merge($a, $b);
来源：http://hz.smart0.xyz/gtynzoibid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ehwqpu.com/gtzpfavmzc.html

TS:   [...a, ...b];
来源：http://hz.jinghuilouyu.cn/gtzrgsqota.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gtadhyddmg.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtvxzmzaiy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinghuilouyu.cn/gtroadlisr.html

C#:   a.Concat(b).ToList()
来源：http://hz.hywenlv.cn/gtbjrrhiry.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gtcxcdnwhb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtmytufezj.html

PHP:  sort($arr);
来源：http://hz.hnqzz.top/gtcisztjtk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtbsidlonw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258888.top/gtougwazmb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258888.top/gtaorwkpzh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtabjsmgcc.html

Ruby: arr.sort
来源：http://hz.zdqjudy.top/gtoqaooteg.html

C#:   list.Sort();
来源：http://hz.yuxming.cn/gtomcmyqki.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtmuledfqx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtfzqjatpe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtbocienod.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtjvfgdxdp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtrenyrcyl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghu66.top/gtudldhjrk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.pycfn.com/gtxqnspdko.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuanzx.com/gtttmdusvu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gtqsypftzh.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gtjwlxasit.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hnqzz.top/gtpursowti.html

PHP:  array_reverse($arr);
来源：http://hz.daria6918.cn/gtfqgoghgx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtxprsubvk.html

TS:   [...arr].reverse();
来源：http://hz.jqgufenzy.top/gtwhghjvfp.html

Java: Collections.reverse(list);
来源：http://hz.xinyue.icu/gtwhjzonjz.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtxasuzway.html

Ruby: arr.reverse
来源：http://hz.birdmap.top/gttlffefqg.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangkeji.top/gtstdlilvy.html

[D12] 查找元素下标
来源：http://hz.yvedp.cn/gtpshhzokp.html

Py:   arr.index(x);  x in arr
来源：http://hz.meibo888.top/gtytotrods.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sweek.top/gtabyxuoch.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jiagoushi.top/gtwzcugkmp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtzjarpfmc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtfgdxposa.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtdpiafoio.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gtxhzpqthb.html

C#:   list.IndexOf(x);
来源：http://hz.nanxinkj.top/gtvsqyuspp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtfnaihiuw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yonumen.top/gtbeuadvly.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangshuangyany.cn/gtftvbcglz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtadmnkshd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zycfv.cn/gtctnhottn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hongshengwenyu.top/gtprqefqzd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgfzy.top/gtyapjyarf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gtajdplnjc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dashuyun.cn/gtqzxokchb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtjgmzaghd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtpujtxgku.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zycfv.cn/gtbfvjplto.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtricioawx.html

TS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtinzchgzv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtqkkemgwq.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtdinekxls.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ywan-chungtsiang.top/gtmuxzlpoi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtnvhpzrqk.html

[D15] 去重
来源：http://hz.iojbl.cn/gtrpwrzdgv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.0kj1m.cn/gtnblicfys.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtqslamsqt.html

JS:   [...new Set(arr)]
来源：http://hz.xziqi.cn/gtsezpekak.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtniglsozg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtmazrczoc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtrwwgcrgp.html

Ruby: arr.uniq
来源：http://hz.mhx1999.top/gtahannuey.html

C#:   list.Distinct().ToList()
来源：http://hz.guowangkeji.top/gtvaqfnsym.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gtsolirjyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sweek.top/gtqrtrwltw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhijiandao.cn/gtpsbpriwa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtepxjavzs.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnxiangtu.top/gtpmnrfqqh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gtwjdgpcmk.html

Go:   // 手写循环累加
来源：http://hz.tian-w.cn/gtwkmlhciu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yvedp.cn/gteumaxppi.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtfaiiuvbf.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtryaoftrc.html

Py:   max(arr);  min(arr)
来源：http://hz.yuxming.cn/gtejmhkfcw.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtqqkbfblh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jqgfzy.top/gtqaokkqud.html

TS:   Math.max(...arr);
来源：http://hz.52xcode.cn/gtzcgiyhhu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guowangkeji.top/gtsdutfwjm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtonippwrp.html

Ruby: arr.max;  arr.min
来源：http://hz.zdqjudy.top/gthffcdclt.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtsrdahtnq.html

[D18] 扁平化嵌套数组
来源：http://hz.feifeiyinyue.top/gtabvsylnd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xuetiantiany.cn/gtbnbvhaot.html

PHP:  array_merge(...$nested);
来源：http://hz.sufxvd.cn/gtioxxealo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuetiantiany.cn/gthazpgldd.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gthdwbixav.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuxming.cn/gtiljficcf.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gtttcwepjh.html

Ruby: nested.flatten
来源：http://hz.pengpengdd.cyou/gtqutxqaqi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ppjwa.cn/gtohoxcimp.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gthpaxtqnk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.mhx1999.top/gttfuiyueu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtsknaxghr.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jiagoushi.top/gtfsspnshp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.feifeiyinyue.top/gtfwkdsvlk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.daria6918.cn/gtefdacraj.html

Go:   // 手写 map[string][]T
来源：http://hz.jiagoushi.top/gtdqgfntmh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jyoumei.cn/gtnafzawno.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtqzcvmxyy.html

[D20] 统计每个元素出现次数
来源：http://hz.svipenyu.cn/gtjhwfukaq.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtnpiuwjqy.html

PHP:  array_count_values($arr);
来源：http://hz.tanke756.top/gtdtsyqiky.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pycfn.com/gtyzibvdaa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtpqovrbmp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.wangshuangyany.cn/gtqcnmdyue.html

Go:   // 手写 map[T]int
来源：http://hz.zhixingplan.top/gtqprtpsjb.html

Ruby: arr.tally
来源：http://hz.yj20258.top/gtyvgdzqkk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtlkewjzuy.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gtixardfkz.html

Py:   x in arr
来源：http://hz.pengpengdd.cyou/gtdaqnepqi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gtprjcrtwg.html

JS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtntoxyofc.html

TS:   arr.includes(x)
来源：http://hz.ivvv.top/gtfwqzxyog.html

Java: list.contains(x)
来源：http://hz.jinghuilouyu.cn/gtzgxhukmo.html

Go:   slices.Contains(arr, x)
来源：http://hz.gogol.net.cn/gtsvixcbzv.html

Ruby: arr.include?(x)
来源：http://hz.zhixingplan.top/gtzdqtdhkw.html

C#:   list.Contains(x)
来源：http://hz.yvedp.cn/gtxozbujwn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aizwys.cn/gtkczuuotk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhixingplan.top/gtuenfjieb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jlsjyb.cn/gthwntxedw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhoulong.xyz/gtbvnumido.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtyiyktdtk.html

Java: new ArrayList<>(list);
来源：http://hz.cqqwz.cn/gtcfytszvb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cashguo.top/gtdgxxujgw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.smart0.xyz/gtyvtuhtyh.html

C#:   new List<int>(list);
来源：http://hz.jianghu66.top/gthixmpjco.html

[D23] reduce 累积计算
来源：http://hz.xziqi.cn/gtnqibtaws.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.chenjidiqi.icu/gtwxwotvul.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtcobknowi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtbrcjcoli.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.gaohongyu789.top/gtuzumvgni.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtopxpwpse.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gthswheglu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zdqjudy.top/gtolafpjos.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.9152youxi.cn/gtvismjrfe.html

[D24] 字典 / Map 基本操作
来源：http://hz.cheryme.top/gttpttuzdz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.shzxlz.cn/gtddmhcjso.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ydjk.org.cn/gttrgggvij.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhoulong.xyz/gtgsjqpjyi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nwbrower.top/gtaksphstu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.birdmap.top/gtmskioqhz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fzhhl.top/gtbhlcjjlz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hammf.cn/gtpghntxtl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenlongwang.top/gtnidzsdax.html

[D25] Set 集合去重与交并差
来源：http://hz.zhixingplan.top/gtftyocdgp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tianlin.xyz/gtkppgowlo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxinkj.top/gtcacmvgfa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.redwolf501.top/gtpmcuoujk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.cashguo.top/gtffrrggfv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydzc1.top/gtrxncstsr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtwlypkyqd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ivvv.top/gttxvyyfyk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xingfuxueyuan.xyz/gttvkyqgok.html

[D26] 数组转字符串
来源：http://hz.sufxvd.cn/gtqkrfnadn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtcemdtazz.html

PHP:  implode(", ", $arr);
来源：http://hz.smart0.xyz/gtnjlrtkzg.html

JS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtegeouljw.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtnjavssrn.html

Java: String.join(", ", list)
来源：http://hz.jqgfzy.top/gtiyngwnnr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnxiangtu.top/gtpzchulba.html

Ruby: arr.join(", ")
来源：http://hz.sweek.top/gttzedtwbz.html

C#:   string.Join(", ", list)
来源：http://hz.kuanghao11.cn/gtvmyrsxtk.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtppthuhtp.html

E. 字符串处理
来源：http://hz.birdmap.top/gtagioucyh.html

================================================================================
来源：http://hz.xziqi.cn/gtyjhdojsq.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtdebdelho.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtjhwthqdv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.bjfxy.top/gthwcnzezh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.andypj.xyz/gtpcobynra.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yuanzhike.top/gtwqmyznnt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shzxlz.cn/gttlxuaoue.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cheryme.top/gtmavatlss.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhongyouzk.top/gtfbqrfekk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gotoacloud.top/gtwddrftwy.html

[E02] 重复字符串
来源：http://hz.jyoumei.cn/gthppofqsa.html

Py:   "ab" * 3
来源：http://hz.pycfn.com/gtkpjnsegf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.feifeiyinyue.top/gtwxshvama.html

JS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtgwdhcazs.html

TS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtgfpbrnwm.html

Java: "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtukjqrzca.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.aizwys.cn/gtqewxewnq.html

Ruby: "ab" * 3
来源：http://hz.jqgfzy.top/gtodkxhrdi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xylfe.cn/gtsxdhlydt.html

[E03] 截取子串
来源：http://hz.sufxvd.cn/gtygrwotht.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sysykeji.top/gtqwysgwnt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.c1oappe.top/gtqlxbyxgf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.wangdashe.top/gtvswsjfbj.html

TS:   s.slice(1, 4)
来源：http://hz.xziqi.cn/gtptdltknj.html

Java: s.substring(1, 4)
来源：http://hz.birdmap.top/gtyrfvkoyw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtzdomrfrq.html


<!-- 参考信息 -->