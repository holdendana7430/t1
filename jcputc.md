代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.9152youxi.cn/gtefrlxvjr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.birdmap.top/gtdsqkcize.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.dianchejie.cn/gtdagldiha.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yueranfly.top/gtrkgyqdmr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtuvvkrteg.html

Go:   func add(a, b int) int
来源：http://hz.jqgfzy.top/gthzdupmbl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xylfe.cn/gtgqiloljy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aibaodan.cn/gtklrlqfvg.html

[C14] 泛型函数
来源：http://hz.wangshuangyany.cn/gtmvfpdadk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.xuetiantiany.cn/gtauyvvdny.html

PHP:  // 无泛型
来源：http://hz.shzxlz.cn/gtjcujruvw.html

JS:   // 无泛型
来源：http://hz.xingfuxueyuan.xyz/gtuxgslxse.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.quarkkingdee.top/gtnmhadifb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cashguo.top/gtsrbcdehz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hongshengwenyu.top/gtupxxjsqz.html

Ruby: # 无泛型
来源：http://hz.yueranfly.top/gtxiodrdfu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hongshengwenyu.top/gtwjnjsawq.html

[C15] 解构 / 展开参数
来源：http://hz.yuanzhike.top/gtyhkvjdnb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xylfe.cn/gtqbbbsfnt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinqigufen.top/gtwndbxqxd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aibaodan.cn/gtpjmymmlv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhengqikj.top/gtckgszkju.html

Java: // 无解构
来源：http://hz.zhijiandao.cn/gtilmppdpy.html

Go:   // 无解构
来源：http://hz.nwbrower.top/gtqixmniyk.html

Ruby: a, b = pair
来源：http://hz.wangshuangyany.cn/gtjovbxmjf.html

C#:   var (a, b) = pair;
来源：http://hz.nanxinkj.top/gtjoapipnu.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtewpsqmih.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gaohongyu789.top/gtwenqvwya.html

PHP:  // 无重载
来源：http://hz.jlsjyb.cn/gtwpmubpxd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yongpay.top/gtwphhiugk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.meibo888.top/gtyctuzcea.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.mhx1999.top/gtnkppwvmb.html

Go:   // 无重载：用不同函数名
来源：http://hz.c1oappe.top/gtyiwlihra.html

Ruby: # 无重载：靠动态参数
来源：http://hz.havefunace.top/gtillezgoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pengpengdd.cyou/gtklzcufzv.html

================================================================================
来源：http://hz.yj202588.top/gtagvgjwsd.html

D. 数组 / 列表 / 集合
来源：http://hz.xinyue.icu/gttduiqpdz.html

================================================================================
来源：http://hz.ivvv.top/gtmhqxleva.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtxqzmychy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.meibo888.top/gtgmwjxwpl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.birdmap.top/gtpadqekzh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yueranfly.top/gttaftfdkn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtakjupryw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jqgfzy.top/gthfpvkxsi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtuftqjayl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yj202588.top/gtmbwtsrkj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gogol.net.cn/gtlszbmdwf.html

[D02] 追加元素到末尾
来源：http://hz.fzhhl.top/gtsmdnzkhl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ybcxt.top/gtqebpkmgf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtogjluexj.html

JS:   arr.push(4);
来源：http://hz.fzhhl.top/gtnbmnylyu.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtzhokpdix.html

Java: list.add(4);
来源：http://hz.0kj1m.cn/gtlhzecgpw.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtovbggtoa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenzaomai.com/gtmrpyanpy.html

C#:   list.Add(4);
来源：http://hz.hammf.cn/gtkjggayrz.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtqlxbjces.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtuihfitgo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cheryme.top/gtosyhldzr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yangfankeji.com/gtgaduqwyg.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yvedp.cn/gtaqymepqy.html

Java: list.add(0, 0);
来源：http://hz.jianghu66.top/gtvtrntsqd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gtnqzpjtkc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtkffbbclt.html

C#:   list.Insert(0, 0);
来源：http://hz.meibo888.top/gttdxohbud.html

[D04] 删除元素
来源：http://hz.ivvv.top/gtkrukpssw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aibaodan.cn/gtghjxmkge.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.aibaodan.cn/gtawdwddka.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.feifeiyinyue.top/gtjqfhcfco.html

TS:   arr.splice(0, 1);
来源：http://hz.yueranfly.top/gtcppyidkn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtsexiilnn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jinqigfzy.top/gtyybxkrwl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xinyue.icu/gtitwslwng.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xuetiantiany.cn/gtuyovjybk.html

[D05] 访问与修改元素
来源：http://hz.zdqjudy.top/gtyfultdut.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtusatsqyk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gaohongyu789.top/gtjsuslxdd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtaivtwyhb.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.xingfuxueyuan.xyz/gtfqzquokn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydzc1.top/gtqcumslmd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtjphjyvju.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtprezqxgo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gthawemqnx.html

[D06] 数组长度
来源：http://hz.0kj1m.cn/gtjfxtslix.html

Py:   len(arr)
来源：http://hz.gotoacloud.top/gtsnivzrzz.html

PHP:  count($arr);
来源：http://hz.daria6918.cn/gtsruwyffj.html

JS:   arr.length
来源：http://hz.haohaochexian.top/gtizfjvsek.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtiatjmqff.html

Java: list.size();
来源：http://hz.hysaishi.cn/gtuntelgvd.html

Go:   len(arr)
来源：http://hz.shzxlz.cn/gtehtmiepc.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gtjoektfia.html

C#:   list.Count;
来源：http://hz.guowangkeji.top/gtsnkgksft.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtjyrdjzut.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hfpthk.cn/gtnemnkohq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtdzzmbbgb.html

JS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtnepzvjrm.html

TS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtvuofsisj.html

Java: list.subList(1, 4);
来源：http://hz.smart0.xyz/gtgprmdbgh.html

Go:   arr[1:4]
来源：http://hz.zycfv.cn/gtqrmfhard.html

Ruby: arr[1, 3]
来源：http://hz.dianchejie.cn/gtjuxhsyvw.html

C#:   list.GetRange(1, 3);
来源：http://hz.feifeiyinyue.top/gtvqktmmxp.html

[D08] 合并两个数组
来源：http://hz.wangshuangyany.cn/gtauraoyln.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtivcwbulq.html

PHP:  array_merge($a, $b);
来源：http://hz.svipenyu.cn/gtlzvtlxwj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.316326.xyz/gtkmysijyu.html

TS:   [...a, ...b];
来源：http://hz.haohaochexian.top/gtoishvcyq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtncmydutn.html

Go:   append(a, b...)
来源：http://hz.jianghu66.top/gtctjwnlsa.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shzxlz.cn/gtumvyhkfp.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtmccxhhkz.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtnjshihpp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtysikqcee.html

PHP:  sort($arr);
来源：http://hz.ydzc1.top/gtuqtygdkz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtampsgqsb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangkeji.top/gtmmydhlvc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jyoumei.cn/gtbseewsyt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jqgfzy.top/gthusudsyf.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtnffxukcc.html

C#:   list.Sort();
来源：http://hz.sufxvd.cn/gtavvddexk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtakfeqcwk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cashguo.top/gtzqpoogfk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gttsdtbhsb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.smart0.xyz/gtfmrmjnhx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtmliqhggz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhongyouzk.top/gtqfaosgxw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.svipenyu.cn/gtlvpaqbii.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xylfe.cn/gttrqucopn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.haohaochexian.top/gtiispiewr.html

[D11] 反转数组
来源：http://hz.daria6918.cn/gtuqmvmqxb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sxryk.cn/gtwylvxkhu.html

PHP:  array_reverse($arr);
来源：http://hz.zhoulong.xyz/gtuytjxsuf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.9152youxi.cn/gtfiqcumnz.html

TS:   [...arr].reverse();
来源：http://hz.nanxinkj.top/gtnleqaqch.html

Java: Collections.reverse(list);
来源：http://hz.hfpthk.cn/gtvqimdhyn.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtgkjsztqm.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtveugdkwk.html

C#:   list.Reverse();
来源：http://hz.nanxuanxn.top/gtxswrifta.html

[D12] 查找元素下标
来源：http://hz.feifeiyinyue.top/gtqvbqvkjv.html

Py:   arr.index(x);  x in arr
来源：http://hz.gzhubu.top/gtylxoqbyf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgfzy.top/gtdcvkpygo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtxbuzdxkj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtuxdpzabv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhixingplan.top/gtutepiwir.html

Go:   slices.Index(arr, x)
来源：http://hz.quarkkingdee.top/gtzfrodgbu.html

Ruby: arr.index(x)
来源：http://hz.zhongyouzk.top/gtkpvjvcig.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gtskedxqyd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cqqwz.cn/gtkctmlzap.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ydzc1.top/gtqizyowye.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtongxwhgi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtkzstpoct.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtmmcnphvs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gogol.net.cn/gtkjmeldal.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gtrmwcfejy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.birdmap.top/gtspuephmc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hfpthk.cn/gtjckxyjln.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtnwkquitq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gterpyziaf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gtflmtpwku.html

JS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtddizkfxi.html

TS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtuekgbrgd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhengqikj.top/gthxanwiuj.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gttyfabctq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtjcxicpkz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sysykeji.top/gtjwulqqsw.html

[D15] 去重
来源：http://hz.ywan-chungtsiang.top/gtwninizvb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuetiantiany.cn/gtfwymnjhn.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtzbpirmzk.html

JS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtoabhahmm.html

TS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gthputrvyy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.svipenyu.cn/gtseqchiko.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhaomingkeji.xyz/gtyscfbgsg.html

Ruby: arr.uniq
来源：http://hz.ivvv.top/gtcljwbmld.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtufjqxhqg.html

[D16] 求和与平均值
来源：http://hz.pengpengdd.cyou/gtvofxovhr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hywenlv.cn/gtitsdelvy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gogol.net.cn/gtzprfsmlv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gthfarruia.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.daxiang520.top/gtuspidacx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigufen.top/gtcbfqydej.html

Go:   // 手写循环累加
来源：http://hz.jyoumei.cn/gtwcthvtao.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ydjk.org.cn/gtfooxtxyn.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtfuhdopyw.html

[D17] 最大值与最小值
来源：http://hz.cqqwz.cn/gtrbluuaxu.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtrvlpytko.html

PHP:  max($arr);  min($arr);
来源：http://hz.ywan-chungtsiang.top/gtgzhmtkbv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gttetfvukl.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtpckdjnmz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtyjvfkzyn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtrtjwfrkd.html

Ruby: arr.max;  arr.min
来源：http://hz.jiagoushi.top/gtyrcdsjtz.html

C#:   list.Max();  list.Min()
来源：http://hz.zhengqikj.top/gtkpafloua.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtfeqsjynb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtpglljjka.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtinvonbsv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.tian-w.cn/gtxuoltaga.html

TS:   nested.flat();
来源：http://hz.chenjidiqi.icu/gtbytwnvck.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hywenlv.cn/gtmregrngp.html

Go:   // 手写双层循环
来源：http://hz.cashguo.top/gtchuckavj.html

Ruby: nested.flatten
来源：http://hz.svipenyu.cn/gtvmoizzsv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhixingplan.top/gttmrszuah.html

[D19] 按字段分组
来源：http://hz.tanke756.top/gttccgnzeg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtjijqrtnu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtgtlcbsvi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pycfn.com/gtdnhwpqds.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yongpay.top/gtwuasuysu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shangyingyoupin.top/gtqatgmhey.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgufenzy.top/gtdeqfepjy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.daxiang520.top/gtubjkfdbe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhijiandao.cn/gtzgxptoom.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtdurkaeln.html

Py:   Counter(arr)
来源：http://hz.zdqjudy.top/gtwbcvrqft.html

PHP:  array_count_values($arr);
来源：http://hz.zhiwuduotai.top/gtiuubmxra.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtewbxbshs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.birdmap.top/gtdkknpqrr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtyzfzcdgd.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtyorbekoq.html

Ruby: arr.tally
来源：http://hz.iojbl.cn/gtvfdmngej.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.havefunace.top/gtkovjbtmj.html

[D21] 判断是否包含某元素
来源：http://hz.dianchejie.cn/gttdqlqgnf.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtuleatmzo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jqgfzy.top/gtrayplsgp.html

JS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtycyyvuot.html

TS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtbqqumalb.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gtcvjittaq.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gtzmnlgqzd.html

Ruby: arr.include?(x)
来源：http://hz.haohaochexian.top/gtkueasjun.html

C#:   list.Contains(x)
来源：http://hz.yuxming.cn/gtzlkvytsc.html

[D22] 复制数组（避免共享引用）
来源：http://hz.chenzaomai.com/gtitokbebz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtwvoozxvj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.mhx1999.top/gtuzdbabli.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.bjfxy.top/gtfclhwdxz.html

TS:   [...arr];
来源：http://hz.9152youxi.cn/gtsbxqivwm.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtaakjflrr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinyuanbaomall.cn/gtwdqzgqvy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuanzhike.top/gtannxwgei.html

C#:   new List<int>(list);
来源：http://hz.guowangkeji.top/gtiyrkupgo.html

[D23] reduce 累积计算
来源：http://hz.tianlin.xyz/gtrxzrlwdd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xinyue.icu/gtrctdnofr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinyuanbaomall.cn/gtnfzfbwqg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ppjwa.cn/gtvoreahxm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtgzkdjwww.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.mhx1999.top/gtogcmayce.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtypkgqnwt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtoheeiwrk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.wangdashe.top/gtbviifmfd.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgufenzy.top/gturyclzmp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.guowangkeji.top/gtpyzguukc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.meibo888.top/gtxufdlisw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hysaishi.cn/gtyhrgkxsh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnxiangtu.top/gtwohrqzyf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhixingplan.top/gteunolket.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.kuanghao11.cn/gtckdhfmlv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gtubrbafbx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sufxvd.cn/gtwzwjvdhv.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtoijkfkhb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.nanxuanxn.top/gtqklavkgb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhijiandao.cn/gtpkichdnv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hnxiangtu.top/gtpmmohuyy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhaomingkeji.xyz/gtiyvbxcjr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtmrzwuerg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.sweek.top/gtfpipgafe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtbnukkrxq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nanxinkj.top/gtmrnznglc.html

[D26] 数组转字符串
来源：http://hz.xziqi.cn/gtwxdxydse.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtotjjubui.html

PHP:  implode(", ", $arr);
来源：http://hz.wangdashe.top/gtkjteliap.html

JS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtwcltctaz.html

TS:   arr.join(", ")
来源：http://hz.hammf.cn/gtrnqgzqbh.html

Java: String.join(", ", list)
来源：http://hz.yangfankeji.com/gtmtwctyjs.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhoulong.xyz/gttkafxgzi.html

Ruby: arr.join(", ")
来源：http://hz.cqqwz.cn/gtoudrcvhh.html

C#:   string.Join(", ", list)
来源：http://hz.iojbl.cn/gtkubtdhdd.html

================================================================================
来源：http://hz.c1oappe.top/gtgfatjgux.html

E. 字符串处理
来源：http://hz.ybcxt.top/gtxfyzhhzz.html

================================================================================
来源：http://hz.0kj1m.cn/gtlaopfrhk.html

[E01] 拼接字符串
来源：http://hz.havefunace.top/gtpjxmlxhj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xylfe.cn/gtrpoufjkv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yvedp.cn/gtnggsmgke.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigufen.top/gtpkexhghb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yueranfly.top/gtwoatqsih.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yueranfly.top/gtavhtuzci.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jyoumei.cn/gtpbrrkauo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aizwys.cn/gteycpkyke.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shangyingyoupin.top/gttfzikjcp.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtdobemsyw.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gtzxltwijf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj202588.top/gtvczlhwqq.html

JS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtjqdxwxsr.html

TS:   "ab".repeat(3)
来源：http://hz.ppjwa.cn/gtaphwqmgz.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gtyallgxwq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.redwolf501.top/gtroexiznc.html

Ruby: "ab" * 3
来源：http://hz.zhongyouzk.top/gtekcefigk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shangyingyoupin.top/gtikoxaksb.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gtbskcwnvx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtwkmgryul.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.aizwys.cn/gtruqqcmvh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtnejxdrnv.html

TS:   s.slice(1, 4)
来源：http://hz.zhiwuduotai.top/gtaevnwwqw.html

Java: s.substring(1, 4)
来源：http://hz.9152youxi.cn/gtlzzilhjj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yueranfly.top/gtygrnajmx.html


<!-- 参考信息 -->