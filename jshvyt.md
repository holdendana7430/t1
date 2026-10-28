代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.hywenlv.cn/gtnqeurzdy.html

Ruby: -> { puts "run" }.call
来源：http://hz.sufxvd.cn/gtylhfofed.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ydjk.org.cn/gtflhfriro.html

[C13] 类型声明 / 类型注解
来源：http://hz.smart0.xyz/gtircwjpnc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.andypj.xyz/gtfxftsjim.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sysykeji.top/gtjhoclwdi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.aibaodan.cn/gtqfuunyne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtoglkrauw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aizwys.cn/gtwqutuxas.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtrejkxjbo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yueranfly.top/gtxyoswjnv.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yongpay.top/gtppavhoek.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gtfqtahvno.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sufxvd.cn/gtjfnmyvau.html

PHP:  // 无泛型
来源：http://hz.haohaochexian.top/gteycmlhur.html

JS:   // 无泛型
来源：http://hz.aibaodan.cn/gtqzmlqxoq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydjk.org.cn/gtpycizmuf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gtzjkewcok.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.9152youxi.cn/gtzdxywcxd.html

Ruby: # 无泛型
来源：http://hz.jianghu66.top/gtlhzrdeql.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.iojbl.cn/gtwcqdnuuc.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtzorybcin.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aibaodan.cn/gtmeutixja.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhoulong.xyz/gthogpvway.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtxcicncyb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sufxvd.cn/gtlrustbxp.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtyirvkudr.html

Go:   // 无解构
来源：http://hz.cucudq.cn/gtgndrwokv.html

Ruby: a, b = pair
来源：http://hz.zhixingplan.top/gtacvubabg.html

C#:   var (a, b) = pair;
来源：http://hz.wangshuangyany.cn/gtripfhtmp.html

[C16] 函数 / 方法重载
来源：http://hz.nwbrower.top/gtvcujmyer.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yueranfly.top/gtpcgffgph.html

PHP:  // 无重载
来源：http://hz.chenlongwang.top/gtaobagekz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtqihcavjl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daxiang520.top/gtppilange.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtdyxfgpap.html

Go:   // 无重载：用不同函数名
来源：http://hz.nanxinkj.top/gtdwyqagju.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtytmhcrwt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtkrdjpndp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtqfycmruc.html

D. 数组 / 列表 / 集合
来源：http://hz.daria6918.cn/gtwrfxzgrh.html

================================================================================
来源：http://hz.jqgufenzy.top/gtutshlcim.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gthqvcswly.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yanxiufei.cn/gtfqdwhtgz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtkbvaybyp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gttallpfpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nanxinkj.top/gtcrdrckbj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuetiantiany.cn/gtywqfmzfi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cashguo.top/gteejrtsqh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangtech.top/gtpsajmjcn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.quarkkingdee.top/gtvuscoeon.html

[D02] 追加元素到末尾
来源：http://hz.zhaomingkeji.xyz/gtzegjbxqs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hfpthk.cn/gtdhrdoxdw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.mhx1999.top/gtojkuolsd.html

JS:   arr.push(4);
来源：http://hz.hywenlv.cn/gtaxhhtzyf.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtkauitjvd.html

Java: list.add(4);
来源：http://hz.haohaochexian.top/gtxyzcxrkq.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgfzy.top/gttpzhjogv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.haohaochexian.top/gtaxkallvp.html

C#:   list.Add(4);
来源：http://hz.shanyushiyangtech.top/gtplwggvin.html

[D03] 在指定位置插入元素
来源：http://hz.meibo888.top/gtfzxmzvyz.html

Py:   arr.insert(0, 0)
来源：http://hz.vqdsnc.cn/gtsoyepkve.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jyoumei.cn/gtvjpfyasv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gthfpuptht.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ppjwa.cn/gtngnljppv.html

Java: list.add(0, 0);
来源：http://hz.andypj.xyz/gtzuubsjja.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sxryk.cn/gtyddnlzxg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.tian-w.cn/gtyghvbrol.html

C#:   list.Insert(0, 0);
来源：http://hz.sufxvd.cn/gtwkbvgntb.html

[D04] 删除元素
来源：http://hz.nanxinkj.top/gtfdwrutsn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.9152youxi.cn/gttrydjmec.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yonumen.top/gtwdnzqgdw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shanyushiyangtech.top/gtvkwwcvms.html

TS:   arr.splice(0, 1);
来源：http://hz.hnqzz.top/gtfujlwazy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ivvv.top/gtahcjvuia.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenlongwang.top/gtocmjwkjx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtqkkhasaf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gtftbqjzal.html

[D05] 访问与修改元素
来源：http://hz.bjfxy.top/gthmgyctgp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtmmlboioa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guowangkeji.top/gthstoojtv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.9152youxi.cn/gtzruzybna.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sysykeji.top/gtipahkiak.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yanxiufei.cn/gtiboxbenh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.bjfxy.top/gtboyxliph.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cheryme.top/gtatphkocy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.guannengcc.top/gtzgjxsmjk.html

[D06] 数组长度
来源：http://hz.chenjidiqi.icu/gtlrymbebf.html

Py:   len(arr)
来源：http://hz.zycfv.cn/gtvtxzoulg.html

PHP:  count($arr);
来源：http://hz.shanyushiyangkeji.top/gtkaebenos.html

JS:   arr.length
来源：http://hz.smart0.xyz/gtsjawdvye.html

TS:   arr.length
来源：http://hz.snrcjt.cn/gtknogwduk.html

Java: list.size();
来源：http://hz.hfpthk.cn/gtztmixysi.html

Go:   len(arr)
来源：http://hz.hysaishi.cn/gtzsubuvhr.html

Ruby: arr.length; arr.size
来源：http://hz.pycfn.com/gtactslzaa.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtctqcghef.html

[D07] 切片 / 取子数组
来源：http://hz.daxiang520.top/gtoajzmazx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtykxzqsmz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.316326.xyz/gtsevsihph.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtxqlxjugr.html

TS:   arr.slice(1, 4);
来源：http://hz.yonumen.top/gtwhkwtdyi.html

Java: list.subList(1, 4);
来源：http://hz.c1oappe.top/gtreiyygax.html

Go:   arr[1:4]
来源：http://hz.jqgfzy.top/gtukqwdisa.html

Ruby: arr[1, 3]
来源：http://hz.daria6918.cn/gtnrbfqjxk.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydzc1.top/gtukqccwpr.html

[D08] 合并两个数组
来源：http://hz.dashuyun.cn/gtqgztfbrd.html

Py:   a + b;  a.extend(b)
来源：http://hz.pengpengdd.cyou/gtixeqwzqj.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gtsltytjth.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gtqlftivis.html

TS:   [...a, ...b];
来源：http://hz.cheryme.top/gtpqmmhnyv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zdqjudy.top/gtoqxgkcyl.html

Go:   append(a, b...)
来源：http://hz.andypj.xyz/gtkpxhqjqx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtpvtiovlq.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuanzx.com/gtdeeqyfba.html

[D09] 排序（升序）
来源：http://hz.guowangkeji.top/gtyhrrlori.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtuktqqihr.html

PHP:  sort($arr);
来源：http://hz.ydjk.org.cn/gthgmmabip.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.aibaodan.cn/gtwhiwroiq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shanyushiyangkeji.top/gtyhoyjvds.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinqigfzy.top/gtknpplmin.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yonumen.top/gtsycukbld.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtlonampnl.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gtjodaabsl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gtlckxlsju.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.wangshuangyany.cn/gtfstfzgnw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxinkj.top/gtnwmbtomt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtqgmqosuv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gtynfzduic.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtvituooxi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tian-w.cn/gtdlrptshe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtuttrdguy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtjuqyoulr.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtfqbqbizk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtzsxjfymf.html

PHP:  array_reverse($arr);
来源：http://hz.zdqjudy.top/gtwxsrkils.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangtech.top/gtbrudhoki.html

TS:   [...arr].reverse();
来源：http://hz.yanxiufei.cn/gtfjpjmlqv.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtcukwhenx.html

Go:   slices.Reverse(arr)
来源：http://hz.pycfn.com/gtchxjujgu.html

Ruby: arr.reverse
来源：http://hz.xingfuxueyuan.xyz/gtalblqjvh.html

C#:   list.Reverse();
来源：http://hz.mhx1999.top/gthscmwryf.html

[D12] 查找元素下标
来源：http://hz.ppjwa.cn/gtdufcueup.html

Py:   arr.index(x);  x in arr
来源：http://hz.yueranfly.top/gtetwstiio.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cheryme.top/gtnnicncck.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jyoumei.cn/gtywwlybym.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gtnvaeffzx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hammf.cn/gthztvrwrf.html

Go:   slices.Index(arr, x)
来源：http://hz.gzhubu.top/gthumgnfan.html

Ruby: arr.index(x)
来源：http://hz.sxryk.cn/gtoqxhnmze.html

C#:   list.IndexOf(x);
来源：http://hz.gogol.net.cn/gtzuedyznx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.wangdashe.top/gtlpefpyfp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangshuangyany.cn/gtiatksbfx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtqeaedfop.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtiknreuai.html

TS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtblsomkac.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.wangdashe.top/gtlpuwcxgu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shzxlz.cn/gtsjrfbwih.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yongpay.top/gtyfhacuqp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gtvhndhxin.html

[D14] 映射转换（每个元素变形）
来源：http://hz.aibaodan.cn/gtuuzaqywl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shzxlz.cn/gtnpddtccw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.9152youxi.cn/gtxzpuasgn.html

JS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtedezamna.html

TS:   arr.map(x => x * 2)
来源：http://hz.shuidangran.top/gtehnfwmhu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tanke756.top/gtpvztwnyi.html

Go:   // 手写循环
来源：http://hz.redwolf501.top/gtuwhemaww.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtgnamxitn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuetiantiany.cn/gtnflfbqjc.html

[D15] 去重
来源：http://hz.aizwys.cn/gtflwaopcv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shzxlz.cn/gtkayybggb.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtbjgmqfxn.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtjlujzfwk.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gttanrjkkv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sweek.top/gtxveoyuuk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.cucudq.cn/gtjflenzqv.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtiumajpoy.html

C#:   list.Distinct().ToList()
来源：http://hz.shanyushiyangkeji.top/gtlmhvicwt.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtmfvnfemt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.andypj.xyz/gtlzvolxzo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtudgdrdld.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtwlsgssmz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtuphxmhyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cheryme.top/gthoclcmvr.html

Go:   // 手写循环累加
来源：http://hz.gotoacloud.top/gtlzdafqby.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sysykeji.top/gttiglzdiv.html

C#:   list.Sum();  list.Average()
来源：http://hz.sxryk.cn/gtcplsgzoa.html

[D17] 最大值与最小值
来源：http://hz.yuanzhike.top/gtfyljemlq.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtdqbsaqmn.html

PHP:  max($arr);  min($arr);
来源：http://hz.feifeiyinyue.top/gtyfubcxtb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tanke756.top/gtgxgfwpta.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gtwnprhiul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ybcxt.top/gtjmugmjlk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtdirnevtt.html

Ruby: arr.max;  arr.min
来源：http://hz.c1oappe.top/gtggvvktia.html

C#:   list.Max();  list.Min()
来源：http://hz.guannengcc.top/gtahdrztte.html

[D18] 扁平化嵌套数组
来源：http://hz.zdqjudy.top/gtialrzgjd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.guannengcc.top/gtigwoxyuk.html

PHP:  array_merge(...$nested);
来源：http://hz.jianghu66.top/gtgmiwiubn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nwbrower.top/gtblqwgrqw.html

TS:   nested.flat();
来源：http://hz.jqgufenzy.top/gtunmcyrwd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yueranfly.top/gtbeehdcot.html

Go:   // 手写双层循环
来源：http://hz.yvedp.cn/gttlyawokd.html

Ruby: nested.flatten
来源：http://hz.xuanzx.com/gtmrtiabxi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.tian-w.cn/gtmbcmpaeg.html

[D19] 按字段分组
来源：http://hz.jinqigfzy.top/gtrukweqyv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtkklgeuis.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aibaodan.cn/gtaxmmgiwb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.kuanghao11.cn/gtjcwtmfwp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.pengpengdd.cyou/gtsithijzq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.fengsongda.top/gtfmixugul.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gthjqxzhdk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fzhhl.top/gtdafzsgnu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jyoumei.cn/gtqegzrdvx.html

[D20] 统计每个元素出现次数
来源：http://hz.hywenlv.cn/gtiwevypjx.html

Py:   Counter(arr)
来源：http://hz.yangfankeji.com/gtvlcbbqpm.html

PHP:  array_count_values($arr);
来源：http://hz.bjfxy.top/gtufzjuhyk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtysbqhnor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.smart0.xyz/gticzwqprz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.daria6918.cn/gthcxqvohd.html

Go:   // 手写 map[T]int
来源：http://hz.shuidangran.top/gtoupdjehk.html

Ruby: arr.tally
来源：http://hz.cucudq.cn/gtynwvnqpy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gthnjfxymc.html

[D21] 判断是否包含某元素
来源：http://hz.316326.xyz/gtwnkzfsqu.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gtjjkbjnen.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtppheetcu.html

JS:   arr.includes(x)
来源：http://hz.jinghuilouyu.cn/gtorizbkqw.html

TS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtzogmdigp.html

Java: list.contains(x)
来源：http://hz.svipenyu.cn/gtlcrfxfth.html

Go:   slices.Contains(arr, x)
来源：http://hz.daria6918.cn/gtpyyvoapg.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtepvzbpfv.html

C#:   list.Contains(x)
来源：http://hz.yuxming.cn/gtbjeuzgze.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cheryme.top/gtqogxsstd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ivvv.top/gtnvxoatvd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gtywqcpozc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gogol.net.cn/gtjlljfilo.html

TS:   [...arr];
来源：http://hz.zhongyouzk.top/gtutmnliyn.html

Java: new ArrayList<>(list);
来源：http://hz.sweek.top/gtdsanwufr.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zycfv.cn/gtwfovoutk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.9152youxi.cn/gtjgeufigx.html

C#:   new List<int>(list);
来源：http://hz.fzhhl.top/gtwucxrmgr.html

[D23] reduce 累积计算
来源：http://hz.ydzc1.top/gtjzcvpwrf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtlmewausr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ydjk.org.cn/gtzaaiddar.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gthmtqzhhd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtdubflhls.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuanzx.com/gtpesqlblr.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtfxcnpsac.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.kuanghao11.cn/gtdnquinwo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigufen.top/gtdciowand.html

[D24] 字典 / Map 基本操作
来源：http://hz.yanxiufei.cn/gtzxzvztvx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sweek.top/gtjfwpgnxh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.bjfxy.top/gtbibhjxqx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.haohaochexian.top/gttxncmevi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.quarkkingdee.top/gtnztavqpb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.xingfuxueyuan.xyz/gtjzesbgqg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cdnleiting.top/gtekbamxgq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yanxiufei.cn/gtbeyilsez.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhoulong.xyz/gtxmjbnhwi.html

[D25] Set 集合去重与交并差
来源：http://hz.fengsongda.top/gtmjsqwbwr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yvedp.cn/gtdqyltizx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yvedp.cn/gtdtnzbjth.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.sysykeji.top/gthxgufzpc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtlhopbdzv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhiwuduotai.top/gtoigxlqyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtnrkytubk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gogol.net.cn/gturpgassw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xylfe.cn/gtghcqsbjs.html

[D26] 数组转字符串
来源：http://hz.zhaomingkeji.xyz/gtsbkzbffi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtgxwadjte.html

PHP:  implode(", ", $arr);
来源：http://hz.hfpthk.cn/gttlkaluko.html

JS:   arr.join(", ")
来源：http://hz.tanke756.top/gtazqwwvib.html

TS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtnhflytzl.html

Java: String.join(", ", list)
来源：http://hz.zycfv.cn/gtiopfsfla.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nwbrower.top/gtjwdacohe.html

Ruby: arr.join(", ")
来源：http://hz.yuanzhike.top/gthymtclsm.html

C#:   string.Join(", ", list)
来源：http://hz.dianchejie.cn/gtjsjlpukl.html

================================================================================
来源：http://hz.hammf.cn/gtaoxosblh.html

E. 字符串处理
来源：http://hz.zycfv.cn/gtdaaxilou.html

================================================================================
来源：http://hz.0kj1m.cn/gtwofhltkk.html

[E01] 拼接字符串
来源：http://hz.jlsjyb.cn/gtnpvysvep.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jianghu66.top/gtooabmidl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhengqikj.top/gtemrremyd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtgulmbdud.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hongshengwenyu.top/gtwjazsmre.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tian-w.cn/gtciijmbzo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gzhubu.top/gtkfgnmamz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aibaodan.cn/gtawxzxudd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhengqikj.top/gttudercvy.html

[E02] 重复字符串
来源：http://hz.wangdashe.top/gtgzbebdfv.html

Py:   "ab" * 3
来源：http://hz.jinqigufen.top/gtonjiqhpm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cqqwz.cn/gtokcdqqkx.html

JS:   "ab".repeat(3)
来源：http://hz.316326.xyz/gtitvybnse.html

TS:   "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtqzvtybok.html

Java: "ab".repeat(3)
来源：http://hz.zhengqikj.top/gtnnwmimda.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.svipenyu.cn/gtifkerzrs.html

Ruby: "ab" * 3
来源：http://hz.chenlongwang.top/gtpcuhbtlu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yuanzhike.top/gtydeuhdwh.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtgozrkytj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yangfankeji.com/gtxwbdcgoe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.sxryk.cn/gtyrshktpl.html


<!-- 参考信息 -->