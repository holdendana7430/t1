代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtfouzgbhf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yonumen.top/gtwqmafubw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenzaomai.com/gtqwlnkrqf.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtddawsscf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yangfankeji.com/gtaffbbubd.html

[C15] 解构 / 展开参数
来源：http://hz.aizwys.cn/gtavxledmx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuanzx.com/gtfqxwduil.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhengqikj.top/gtnicakkxx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtanqmbfjc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guowangkeji.top/gtxdzddppa.html

Java: // 无解构
来源：http://hz.xuetiantiany.cn/gtxnhlexvi.html

Go:   // 无解构
来源：http://hz.aizwys.cn/gtyymxgjep.html

Ruby: a, b = pair
来源：http://hz.zdqjudy.top/gtdrjgnoib.html

C#:   var (a, b) = pair;
来源：http://hz.jinyuanbaomall.cn/gtmomkbkjt.html

[C16] 函数 / 方法重载
来源：http://hz.zhijiandao.cn/gttjezcheh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cheryme.top/gthhozllry.html

PHP:  // 无重载
来源：http://hz.havefunace.top/gtsqqveftq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.sysykeji.top/gttfvtiswb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhixingplan.top/gttlgwbjjo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenjidiqi.icu/gtozivbfdn.html

Go:   // 无重载：用不同函数名
来源：http://hz.52xcode.cn/gtbsrypbug.html

Ruby: # 无重载：靠动态参数
来源：http://hz.feifeiyinyue.top/gtlvrihgbl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.bjfxy.top/gtktypmzui.html

================================================================================
来源：http://hz.sufxvd.cn/gtxtulncxz.html

D. 数组 / 列表 / 集合
来源：http://hz.jlsjyb.cn/gtcqjhowfd.html

================================================================================
来源：http://hz.yj20258888.top/gtmlmgyeqk.html

[D01] 创建数组 / 列表
来源：http://hz.xziqi.cn/gtxdnmiysa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.quarkkingdee.top/gtmqgcmzgs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yongpay.top/gtbcmqudat.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.mhx1999.top/gtggvnwvdk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangdashe.top/gtfcyfbmnm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cdnleiting.top/gtzwopkclc.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fzhhl.top/gtetquyyik.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtzoscaqfw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sufxvd.cn/gteefnroii.html

[D02] 追加元素到末尾
来源：http://hz.chenjidiqi.icu/gtkgukyoqo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gtssmmtgbr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.nwbrower.top/gtrwexkgxg.html

JS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtyfsokwqq.html

TS:   arr.push(4);
来源：http://hz.hammf.cn/gtwmfjigpn.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtwytqljnd.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gtfwewbfqq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangkeji.top/gtovbxpseh.html

C#:   list.Add(4);
来源：http://hz.andypj.xyz/gtylsgrtxb.html

[D03] 在指定位置插入元素
来源：http://hz.yanxiufei.cn/gtwfwiddxg.html

Py:   arr.insert(0, 0)
来源：http://hz.xziqi.cn/gtblpfuatm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pycfn.com/gtzgnioxpq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shangyingyoupin.top/gtvfarjpap.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtxofkdbhz.html

Java: list.add(0, 0);
来源：http://hz.sweek.top/gtsielkfnr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cashguo.top/gttfaifhwk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenjidiqi.icu/gtciykhqtb.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gthqpagqhx.html

[D04] 删除元素
来源：http://hz.hysaishi.cn/gtduiaxvpo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gogol.net.cn/gtmnydolgr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shanyushiyangtech.top/gtoiinpvyn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigufen.top/gtampnvpdw.html

TS:   arr.splice(0, 1);
来源：http://hz.dianchejie.cn/gtrcmmpges.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gotoacloud.top/gtwxysymkb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gteqlnqbvt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.fzhhl.top/gtewddlyxx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.vqdsnc.cn/gtunogagvw.html

[D05] 访问与修改元素
来源：http://hz.zhongyouzk.top/gtmraxfdrm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtgwdkvzdy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yuxming.cn/gtezqmkjlr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fzhhl.top/gtylujqlzs.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zycfv.cn/gttindzmgc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gtahwxdizx.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtnpjzsvtz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtvxwlhsjq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.fengsongda.top/gtzkuzrfqy.html

[D06] 数组长度
来源：http://hz.hammf.cn/gtynajmcbg.html

Py:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtbrgxdcdo.html

PHP:  count($arr);
来源：http://hz.yanxiufei.cn/gtdwgzwgzz.html

JS:   arr.length
来源：http://hz.fengsongda.top/gtmjfxbsrz.html

TS:   arr.length
来源：http://hz.c1oappe.top/gtzsosaeha.html

Java: list.size();
来源：http://hz.yvedp.cn/gtakwtybkj.html

Go:   len(arr)
来源：http://hz.yj20258888.top/gtnwncqxjb.html

Ruby: arr.length; arr.size
来源：http://hz.dashuyun.cn/gthjsgjvap.html

C#:   list.Count;
来源：http://hz.jqgfzy.top/gtfilpifiq.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtrunqnoya.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.smart0.xyz/gtdyxmvbfi.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zdqjudy.top/gtfszofaak.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gtickohzql.html

TS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtjfmwzrps.html

Java: list.subList(1, 4);
来源：http://hz.0kj1m.cn/gthzkzzrvj.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtmmmwqlxp.html

Ruby: arr[1, 3]
来源：http://hz.kuanghao11.cn/gtfbadklof.html

C#:   list.GetRange(1, 3);
来源：http://hz.sysykeji.top/gtfekfpkko.html

[D08] 合并两个数组
来源：http://hz.ydjk.org.cn/gtsrfiprbl.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gtldyqsekw.html

PHP:  array_merge($a, $b);
来源：http://hz.yueranfly.top/gtkaiffput.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tian-w.cn/gtitbysecj.html

TS:   [...a, ...b];
来源：http://hz.iojbl.cn/gtncmmdkin.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gaohongyu789.top/gtrvhjbhzd.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gtymaegasg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenjidiqi.icu/gttkheqmlg.html

C#:   a.Concat(b).ToList()
来源：http://hz.fengsongda.top/gtnwzipcqq.html

[D09] 排序（升序）
来源：http://hz.guowangkeji.top/gtzorilbub.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gtsvzawstr.html

PHP:  sort($arr);
来源：http://hz.zhiwuduotai.top/gtuselmrws.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtszybrtnf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangshuangyany.cn/gtbtvoqigd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.c1oappe.top/gtpzkmyyjh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.meibo888.top/gtwezomflj.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtwpovakqx.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gtkvxaudqu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj202588.top/gtnqpqsdcp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gtinxdkqwx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtiunysjxk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtjtjindbn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtvysrznrt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gzhubu.top/gturayfoys.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtzxjbgiri.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gogol.net.cn/gtgaqanzvo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtiyohwocx.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gtsujeharp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.redwolf501.top/gtzdpbxsjr.html

PHP:  array_reverse($arr);
来源：http://hz.gotoacloud.top/gtclzdpfrq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtajabbovj.html

TS:   [...arr].reverse();
来源：http://hz.cashguo.top/gtnkpuyhoo.html

Java: Collections.reverse(list);
来源：http://hz.pengpengdd.cyou/gtfhejrpne.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtwvdamvxi.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtcyfjagfb.html

C#:   list.Reverse();
来源：http://hz.smart0.xyz/gtwauctniv.html

[D12] 查找元素下标
来源：http://hz.yonumen.top/gtsbydkkcs.html

Py:   arr.index(x);  x in arr
来源：http://hz.xziqi.cn/gthbbkdkfa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.52xcode.cn/gtbppabidx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtedyxxfwc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgufenzy.top/gthjuolgyu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.svipenyu.cn/gtbkkeunti.html

Go:   slices.Index(arr, x)
来源：http://hz.dianchejie.cn/gtnnerkdax.html

Ruby: arr.index(x)
来源：http://hz.feifeiyinyue.top/gtggglnwes.html

C#:   list.IndexOf(x);
来源：http://hz.zhoulong.xyz/gtlcgcaung.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yvedp.cn/gtrucnclig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.vqdsnc.cn/gtlnkcxefk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shanyushiyangkeji.top/gththupmjk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.haohaochexian.top/gtydekppde.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtzhyqcrpa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jinghuilouyu.cn/gtsvoyfzpd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.316326.xyz/gtrdhlchhh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.smart0.xyz/gtessydrsz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigfzy.top/gtglkhrmix.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gthhsdxdyc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hnxiangtu.top/gtdzqghaef.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigfzy.top/gtjfdacaxc.html

JS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gttacetmqj.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinyuanbaomall.cn/gthumgisrp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aibaodan.cn/gtzmznlwfk.html

Go:   // 手写循环
来源：http://hz.quarkkingdee.top/gtlyajvqyo.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtexpiagag.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jqgfzy.top/gtrbyduerw.html

[D15] 去重
来源：http://hz.gzhubu.top/gtxptkxysm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.haohaochexian.top/gtlzwtozts.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtjmlxblmn.html

JS:   [...new Set(arr)]
来源：http://hz.fengsongda.top/gtabysoxsb.html

TS:   [...new Set(arr)]
来源：http://hz.fengsongda.top/gtpfdqcyik.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.bjfxy.top/gttvomuroa.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pycfn.com/gtmynyckfa.html

Ruby: arr.uniq
来源：http://hz.havefunace.top/gtuqmvsbbt.html

C#:   list.Distinct().ToList()
来源：http://hz.zycfv.cn/gtsuafngcy.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtrhxifgcu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj20258888.top/gtwquotdkq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.mhx1999.top/gtcrhzxter.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tanke756.top/gtkxjypyap.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinghuilouyu.cn/gtgmppzbwg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj202588.top/gtplxrprlw.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtgfxbqlua.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgufenzy.top/gtbllikkdr.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtgclqxjjl.html

[D17] 最大值与最小值
来源：http://hz.shzxlz.cn/gtrqrdhake.html

Py:   max(arr);  min(arr)
来源：http://hz.nwbrower.top/gticfiolfe.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gtglfgrodp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cdnleiting.top/gtgmhxdmii.html

TS:   Math.max(...arr);
来源：http://hz.chenlongwang.top/gtqmybgitu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xingfuxueyuan.xyz/gtgvrsbuif.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.redwolf501.top/gtyhxomnhp.html

Ruby: arr.max;  arr.min
来源：http://hz.xinyue.icu/gtasrdhles.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtwpnyhgfd.html

[D18] 扁平化嵌套数组
来源：http://hz.yj20258888.top/gtrcxrnktl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jianghu66.top/gtwchqaqhx.html

PHP:  array_merge(...$nested);
来源：http://hz.316326.xyz/gtqmdddmcq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.feifeiyinyue.top/gtohvuuohj.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtzyshywyb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zdqjudy.top/gttflqijiv.html

Go:   // 手写双层循环
来源：http://hz.cheryme.top/gttypwzvjb.html

Ruby: nested.flatten
来源：http://hz.havefunace.top/gtkfguvzmw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtyxuwnsuc.html

[D19] 按字段分组
来源：http://hz.hongshengwenyu.top/gtkkwzffbs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xuetiantiany.cn/gtsciitbuu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtwetuvxxe.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtagmkznji.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtpyktfwbo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxinkj.top/gtrjmjugrl.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtolfmjcbp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tianlin.xyz/gtvzstncos.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hysaishi.cn/gtkmvxtkau.html

[D20] 统计每个元素出现次数
来源：http://hz.yuxming.cn/gtkkoeqpow.html

Py:   Counter(arr)
来源：http://hz.yuxming.cn/gttpfinmha.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtxdigvtrk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cqqwz.cn/gtvysvfjqt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yueranfly.top/gtfcmtwcdx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.smart0.xyz/gtrodiwhgh.html

Go:   // 手写 map[T]int
来源：http://hz.zhiwuduotai.top/gttgbwljzs.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtszxckdxd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nwbrower.top/gtcqrjwbjj.html

[D21] 判断是否包含某元素
来源：http://hz.zhengqikj.top/gtpwsskids.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtdpzqubqd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhongyouzk.top/gtnjrhakyy.html

JS:   arr.includes(x)
来源：http://hz.fzhhl.top/gtaqjlntig.html

TS:   arr.includes(x)
来源：http://hz.havefunace.top/gtvfizrjfv.html

Java: list.contains(x)
来源：http://hz.bjfxy.top/gtrlmepqyw.html

Go:   slices.Contains(arr, x)
来源：http://hz.ivvv.top/gtxosklzbg.html

Ruby: arr.include?(x)
来源：http://hz.aibaodan.cn/gtenxfepjv.html

C#:   list.Contains(x)
来源：http://hz.yj20258888.top/gtphmhqnar.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tanke756.top/gttxibullm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ydzc1.top/gtjpcnidql.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sweek.top/gtyriwcrzz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydjk.org.cn/gtajfiwvvp.html

TS:   [...arr];
来源：http://hz.ydjk.org.cn/gtatfebgsp.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtjpzejinu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zdqjudy.top/gtpmbsghqd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ppjwa.cn/gtiiluweac.html

C#:   new List<int>(list);
来源：http://hz.yuanzhike.top/gtosnukdxt.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtfazdhint.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.9152youxi.cn/gtpwjrtvqn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gaohongyu789.top/gtbquxhmpr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhaomingkeji.xyz/gtrwbcurdd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yonumen.top/gthonrblay.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtodzijrtm.html

Go:   // 手写循环
来源：http://hz.gotoacloud.top/gtfsygaseg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yueranfly.top/gtsflnkkss.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sweek.top/gtkogttvml.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhaomingkeji.xyz/gtagbmkpcl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.mhx1999.top/gtycnezyjp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtrrjrvlxb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxuanxn.top/gtdtcalsxw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.birdmap.top/gtdmydrwyw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.meibo888.top/gtwswjftyo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtxbmdxvce.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.meibo888.top/gtrjgogjgf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dianchejie.cn/gtecvojhkt.html

[D25] Set 集合去重与交并差
来源：http://hz.cucudq.cn/gtwidphujt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtjivvvrrf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.316326.xyz/gtuelpmzei.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cdnleiting.top/gtyuudrbjv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gthbgoqwed.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daria6918.cn/gtusqwwbnz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhongyouzk.top/gtiyiypulq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.bjfxy.top/gtdntuwcxj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.mhx1999.top/gtcurcwdkw.html

[D26] 数组转字符串
来源：http://hz.shangyingyoupin.top/gtivqezokh.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xingfuxueyuan.xyz/gtgcimtzsf.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgufenzy.top/gtvhgjbkdl.html

JS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gthwxiyzmu.html

TS:   arr.join(", ")
来源：http://hz.nwbrower.top/gtdxescvzz.html

Java: String.join(", ", list)
来源：http://hz.daxiang520.top/gtwkntyohv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jqgfzy.top/gtnbdtvaug.html

Ruby: arr.join(", ")
来源：http://hz.zycfv.cn/gthqgotezm.html

C#:   string.Join(", ", list)
来源：http://hz.gaohongyu789.top/gttnvbbfxa.html

================================================================================
来源：http://hz.jinqigfzy.top/gticcrbhav.html

E. 字符串处理
来源：http://hz.zhijiandao.cn/gtvwwxijtj.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcbucxkqc.html

[E01] 拼接字符串
来源：http://hz.cdnleiting.top/gtuztbjkjw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gthunaklmt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtsnzysrog.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hfpthk.cn/gtlrexwmxi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gotoacloud.top/gtceyxszjg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtxesmwueo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuetiantiany.cn/gtupabtyni.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhengqikj.top/gtnkaendpc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shanyushiyangtech.top/gtdgvlrefy.html

[E02] 重复字符串
来源：http://hz.sysykeji.top/gtujqpsvob.html

Py:   "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtlxuohlaf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hnxiangtu.top/gtsyemqpqf.html

JS:   "ab".repeat(3)
来源：http://hz.daxiang520.top/gttfspejqi.html

TS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtwnzhlewj.html

Java: "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtspizjxkq.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.iojbl.cn/gtlgebsagv.html

Ruby: "ab" * 3
来源：http://hz.fzhhl.top/gtzdyxpcoy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangtech.top/gtlnbcljyi.html

[E03] 截取子串
来源：http://hz.wangdashe.top/gtktmaoadz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhaomingkeji.xyz/gtzdeqgukz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yj20258888.top/gtoxjmmqix.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtzlidmgbj.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gtxlrsplwh.html

Java: s.substring(1, 4)
来源：http://hz.sweek.top/gtnhmtohko.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jiagoushi.top/gtkoihthsq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xylfe.cn/gtowmgdvuq.html

C#:   s.Substring(1, 3)
来源：http://hz.gaohongyu789.top/gthattsuna.html

[E04] 查找子串位置
来源：http://hz.cdnleiting.top/gtyrodpown.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtvaabeand.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gtirrxxdfb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jianghu66.top/gtoxwbxktd.html

TS:   s.indexOf("x")
来源：http://hz.hysaishi.cn/gtavgtpdip.html

Java: s.indexOf("x")
来源：http://hz.xinyue.icu/gtjuopivej.html

Go:   strings.Index(s, "x")
来源：http://hz.hammf.cn/gtksyowlnu.html

Ruby: s.index("x")
来源：http://hz.birdmap.top/gtzzrkwlsf.html

C#:   s.IndexOf("x")
来源：http://hz.gotoacloud.top/gtywkalxaf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gttieddnax.html


<!-- 参考信息 -->