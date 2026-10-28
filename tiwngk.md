代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zycfv.cn/gtewhaxdgt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtujoowrsy.html

Java: // 无解构
来源：http://hz.zhixingplan.top/gtdxycyhop.html

Go:   // 无解构
来源：http://hz.xuanzx.com/gtvmvtvayr.html

Ruby: a, b = pair
来源：http://hz.hfpthk.cn/gtrwpjquvh.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gtadtnbqjf.html

[C16] 函数 / 方法重载
来源：http://hz.zhiwuduotai.top/gtwcmzmhvx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gaohongyu789.top/gtjtwyncmw.html

PHP:  // 无重载
来源：http://hz.andypj.xyz/gtrahwxiig.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gaohongyu789.top/gtnlitigtp.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.shanyushiyangtech.top/gtdzhwrqzo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xinyue.icu/gtgzwknxqf.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtwjpvxjea.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxinkj.top/gtzvqpcovy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cucudq.cn/gtjfdglowx.html

================================================================================
来源：http://hz.zdqjudy.top/gtamkwesfz.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtkkmjzhia.html

================================================================================
来源：http://hz.gogol.net.cn/gtxdztbjso.html

[D01] 创建数组 / 列表
来源：http://hz.feifeiyinyue.top/gtavggdlrp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.haohaochexian.top/gtnllivonu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gzhubu.top/gtchnbggtk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yueranfly.top/gtqdvxocaq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtvsenmlzz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jiagoushi.top/gtnguxqvcs.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.snrcjt.cn/gthorwigac.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pengpengdd.cyou/gteunphltm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtcymbpllx.html

[D02] 追加元素到末尾
来源：http://hz.shuidangran.top/gtqrnsvqyl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daria6918.cn/gtkoikvrax.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenjidiqi.icu/gtvgopcdmf.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtfsvkvrxi.html

TS:   arr.push(4);
来源：http://hz.ydjk.org.cn/gtzyhigkjj.html

Java: list.add(4);
来源：http://hz.bjfxy.top/gtsmlywsaj.html

Go:   arr = append(arr, 4)
来源：http://hz.nwbrower.top/gtjlqongml.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yj202588.top/gtajehsmuo.html

C#:   list.Add(4);
来源：http://hz.mhx1999.top/gtgpbnrguk.html

[D03] 在指定位置插入元素
来源：http://hz.aizwys.cn/gtwfmmwwkt.html

Py:   arr.insert(0, 0)
来源：http://hz.guowangkeji.top/gtnpclyyqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aizwys.cn/gtznloshbg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuxming.cn/gtyjvsnpyi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xylfe.cn/gtizcmobxc.html

Java: list.add(0, 0);
来源：http://hz.hywenlv.cn/gtuwpatron.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.pycfn.com/gteozkgnzl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gttwhhzapn.html

C#:   list.Insert(0, 0);
来源：http://hz.jyoumei.cn/gtaolotouv.html

[D04] 删除元素
来源：http://hz.jqgufenzy.top/gtzgqncawu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.haohaochexian.top/gtyapslbpr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gtdckffere.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.aizwys.cn/gtwxcmgjin.html

TS:   arr.splice(0, 1);
来源：http://hz.52xcode.cn/gteiqdjtwi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtoyaildyn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.quarkkingdee.top/gtzlgxunlw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jinqigufen.top/gtlgbjhazt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nwbrower.top/gtwtrltwcj.html

[D05] 访问与修改元素
来源：http://hz.sufxvd.cn/gtkpoctkvz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnqzz.top/gtldixldom.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtcyfavflh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.snrcjt.cn/gtsflcqvqg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangshuangyany.cn/gtfcltrxsf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuxming.cn/gtiiojdhcd.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtvneqzyis.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gtvzvroryl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hammf.cn/gtcwwbtmkj.html

[D06] 数组长度
来源：http://hz.52xcode.cn/gtyleuycrm.html

Py:   len(arr)
来源：http://hz.aibaodan.cn/gtnijsjumq.html

PHP:  count($arr);
来源：http://hz.fzhhl.top/gtgxvycbkq.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtnlftxtxa.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtqauelcnv.html

Java: list.size();
来源：http://hz.jinqigufen.top/gtrzvdxbxn.html

Go:   len(arr)
来源：http://hz.cucudq.cn/gtpdrjzanj.html

Ruby: arr.length; arr.size
来源：http://hz.yongpay.top/gtmajacued.html

C#:   list.Count;
来源：http://hz.shzxlz.cn/gtoobhtgcp.html

[D07] 切片 / 取子数组
来源：http://hz.xuetiantiany.cn/gthjyodwas.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.chenjidiqi.icu/gtrxjeifdo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenlongwang.top/gtavweidma.html

JS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtjvdamfyb.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtyoiykckx.html

Java: list.subList(1, 4);
来源：http://hz.aibaodan.cn/gtcmfkngfj.html

Go:   arr[1:4]
来源：http://hz.yuxming.cn/gtywfswect.html

Ruby: arr[1, 3]
来源：http://hz.bjfxy.top/gtgczspeyi.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxuanxn.top/gtaugdahgx.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtzcttrpxu.html

Py:   a + b;  a.extend(b)
来源：http://hz.xylfe.cn/gtxhztaeiu.html

PHP:  array_merge($a, $b);
来源：http://hz.dianchejie.cn/gteikxrluv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dianchejie.cn/gtypaolnhe.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtzdddfdlm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtxpicemos.html

Go:   append(a, b...)
来源：http://hz.hammf.cn/gtagnslmhp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxinkj.top/gtndnaweuf.html

C#:   a.Concat(b).ToList()
来源：http://hz.kuanghao11.cn/gtckwrnyic.html

[D09] 排序（升序）
来源：http://hz.yj202588.top/gtcrcqgttm.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yuanzhike.top/gtzdeswepz.html

PHP:  sort($arr);
来源：http://hz.daxiang520.top/gtnrcnzbnm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hongshengwenyu.top/gtzpignzio.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gtjdkwstuu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gttychpodc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xziqi.cn/gtshmbbosr.html

Ruby: arr.sort
来源：http://hz.shuidangran.top/gtqfadiyvj.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtjyrlxsqo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.daxiang520.top/gtssbsoppf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.svipenyu.cn/gtopikzogs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hnqzz.top/gtgmuofdwv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtevyzfnog.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gthrpxgezx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtjjxoqgmw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtxsjhaepu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxuanxn.top/gtnkfblaso.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtlyuzvzze.html

[D11] 反转数组
来源：http://hz.hongshengwenyu.top/gtjucxdozv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtuwcpddcf.html

PHP:  array_reverse($arr);
来源：http://hz.hongshengwenyu.top/gtlygmknie.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tian-w.cn/gtvaegfokx.html

TS:   [...arr].reverse();
来源：http://hz.nwbrower.top/gtcausugxu.html

Java: Collections.reverse(list);
来源：http://hz.zhiwuduotai.top/gtorqtsmpp.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigfzy.top/gtgdgcoxzg.html

Ruby: arr.reverse
来源：http://hz.andypj.xyz/gtodxjpvwd.html

C#:   list.Reverse();
来源：http://hz.haohaochexian.top/gtebybmfip.html

[D12] 查找元素下标
来源：http://hz.jinqigfzy.top/gtcyrcrerm.html

Py:   arr.index(x);  x in arr
来源：http://hz.sufxvd.cn/gtwvwjkytl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tanke756.top/gtqvasjyhd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtppqeryol.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shangyingyoupin.top/gtgsgrqxee.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.kuanghao11.cn/gtwkbomjvp.html

Go:   slices.Index(arr, x)
来源：http://hz.shuidangran.top/gttsfabnqa.html

Ruby: arr.index(x)
来源：http://hz.shangyingyoupin.top/gtopagiwez.html

C#:   list.IndexOf(x);
来源：http://hz.gotoacloud.top/gtcucvbzwc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yj202588.top/gtahedzfww.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.52xcode.cn/gtzlttyxfx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtauyupugk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gogol.net.cn/gtutzgavcz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtgeuxehef.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.feifeiyinyue.top/gtjwtuaocx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtaaaesmcw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtvzirfuyh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yj20258.top/gtxmuspysk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtaszjlhmu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xingfuxueyuan.xyz/gtquhitxaz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtqwqqvmmp.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangkeji.top/gtwukbxvya.html

TS:   arr.map(x => x * 2)
来源：http://hz.jyoumei.cn/gtlukcfgzb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.guannengcc.top/gtkfowvlra.html

Go:   // 手写循环
来源：http://hz.jinghuilouyu.cn/gtutoacmie.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ybcxt.top/gtcbltbhyu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gttnyhsoxa.html

[D15] 去重
来源：http://hz.pycfn.com/gttpdltkcf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.svipenyu.cn/gtaifgejge.html

PHP:  array_unique($arr);
来源：http://hz.yangfankeji.com/gtparxqhpe.html

JS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtuuvupxfm.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtewhdsyfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.c1oappe.top/gtmwjmgorc.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gtkdelyyxi.html

Ruby: arr.uniq
来源：http://hz.nwbrower.top/gtcslworxp.html

C#:   list.Distinct().ToList()
来源：http://hz.kuanghao11.cn/gtzixbdcjx.html

[D16] 求和与平均值
来源：http://hz.chenlongwang.top/gtljlaebkc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.feifeiyinyue.top/gtlkeifhre.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ywan-chungtsiang.top/gtcmdbpalz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtliyajvlp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gtfrrcluds.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cashguo.top/gtzxqsadcc.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gtqudkmdml.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nwbrower.top/gtefocbhcf.html

C#:   list.Sum();  list.Average()
来源：http://hz.fengsongda.top/gthtuafqyr.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtugbycqgi.html

Py:   max(arr);  min(arr)
来源：http://hz.yuanzhike.top/gtxfahxmgv.html

PHP:  max($arr);  min($arr);
来源：http://hz.gotoacloud.top/gtpjmtxbef.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.chenzaomai.com/gtogutayaj.html

TS:   Math.max(...arr);
来源：http://hz.tanke756.top/gtmglrkksa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shuidangran.top/gtxoiouzpf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtxkocowuk.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtljkepnby.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gthqiutulf.html

[D18] 扁平化嵌套数组
来源：http://hz.guannengcc.top/gtbwqtuwjh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yangfankeji.com/gtvktbpauq.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtizyoehel.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj202588.top/gtgqeotrjf.html

TS:   nested.flat();
来源：http://hz.jyoumei.cn/gtjmaxzoox.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtwratffzg.html

Go:   // 手写双层循环
来源：http://hz.cucudq.cn/gtmvmyqxjf.html

Ruby: nested.flatten
来源：http://hz.haohaochexian.top/gtwcrlnqnt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtmyizsmgt.html

[D19] 按字段分组
来源：http://hz.havefunace.top/gtosnvszob.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hongshengwenyu.top/gtjbhambwc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xuetiantiany.cn/gtzpejkhuo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gttthefjex.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtyhwxcbjr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigfzy.top/gtckbdrfqq.html

Go:   // 手写 map[string][]T
来源：http://hz.guannengcc.top/gtxpkkaobt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.bjfxy.top/gteezzhdwm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtdsfxyfbj.html

[D20] 统计每个元素出现次数
来源：http://hz.sweek.top/gtzvhyewzf.html

Py:   Counter(arr)
来源：http://hz.nwbrower.top/gtisdfzoof.html

PHP:  array_count_values($arr);
来源：http://hz.zhoulong.xyz/gtopcqygow.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.nanxuanxn.top/gtqblsolku.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sweek.top/gtvdnutvot.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.52xcode.cn/gtixsgieqe.html

Go:   // 手写 map[T]int
来源：http://hz.hywenlv.cn/gteygfckzm.html

Ruby: arr.tally
来源：http://hz.xuanzx.com/gtejdffbol.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.smart0.xyz/gtctbqsjxt.html

[D21] 判断是否包含某元素
来源：http://hz.jinghuilouyu.cn/gtpdkpavsn.html

Py:   x in arr
来源：http://hz.ivvv.top/gtfrhzfnhp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.dianchejie.cn/gtmtpikiga.html

JS:   arr.includes(x)
来源：http://hz.meibo888.top/gtvdyelolb.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gthfkmwtuk.html

Java: list.contains(x)
来源：http://hz.yvedp.cn/gtveieupia.html

Go:   slices.Contains(arr, x)
来源：http://hz.gzhubu.top/gtfqrxjsyz.html

Ruby: arr.include?(x)
来源：http://hz.tianlin.xyz/gtbdrhorce.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtyvwsjimu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtsdjfnuog.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gotoacloud.top/gtzorwbizy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cdnleiting.top/gtyobgagfa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gtybaeccnh.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtvqywmxte.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtdijeliqm.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shzxlz.cn/gticzxdmvo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.52xcode.cn/gtkjpbrkrx.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtlaqhgews.html

[D23] reduce 累积计算
来源：http://hz.sweek.top/gttnaaxipw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cucudq.cn/gtpxjcodud.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhaomingkeji.xyz/gtkxoezfej.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.pengpengdd.cyou/gtaclnkawu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jqgufenzy.top/gtqbyetufg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jyoumei.cn/gtogwjdaex.html

Go:   // 手写循环
来源：http://hz.zhoulong.xyz/gtvvpqrwor.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.fzhhl.top/gtigfjahrl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aizwys.cn/gttalcrlvj.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydzc1.top/gtsdwskdvv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangdashe.top/gtujwuvmpx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtptjtrxxf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gtkrfwlobc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.tian-w.cn/gttuvtfssk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtgpkmrnwv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yj20258888.top/gthqbvnddq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xylfe.cn/gtirjgvktn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.guannengcc.top/gtzepduspx.html

[D25] Set 集合去重与交并差
来源：http://hz.ppjwa.cn/gthsnuqoah.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ybcxt.top/gtbwmdelsv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ybcxt.top/gtetvabmbj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xuetiantiany.cn/gtehlukexa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dianchejie.cn/gtapdoovqx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gttmsymihp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtdqdlswaa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtvnknuiin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gotoacloud.top/gtcutpbssc.html

[D26] 数组转字符串
来源：http://hz.snrcjt.cn/gtlqqbjhcz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ywan-chungtsiang.top/gtnjarebwe.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gtoipopbxi.html

JS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtoprcxord.html

TS:   arr.join(", ")
来源：http://hz.chenjidiqi.icu/gtexnpoyem.html

Java: String.join(", ", list)
来源：http://hz.ehwqpu.com/gtvwvgdhht.html

Go:   strings.Join(strs, ", ")
来源：http://hz.vqdsnc.cn/gtcdpienyu.html

Ruby: arr.join(", ")
来源：http://hz.hnqzz.top/gthnhgwrft.html

C#:   string.Join(", ", list)
来源：http://hz.andypj.xyz/gtjonregpd.html

================================================================================
来源：http://hz.guowangkeji.top/gtjnkytdwt.html

E. 字符串处理
来源：http://hz.yangfankeji.com/gtiqarroag.html

================================================================================
来源：http://hz.ydzc1.top/gtgcvbucpb.html

[E01] 拼接字符串
来源：http://hz.fengsongda.top/gtslwbdyhj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ywan-chungtsiang.top/gtlqhzibfd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.dianchejie.cn/gtorsccxdx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gttgportxs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtvwtchfwp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtvlawnzte.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.quarkkingdee.top/gtxiupersg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xinyue.icu/gtnwppbroh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtsynqafbt.html

[E02] 重复字符串
来源：http://hz.jqgufenzy.top/gtbvrhhtaq.html

Py:   "ab" * 3
来源：http://hz.316326.xyz/gtygtnfysa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yvedp.cn/gtvrwzukep.html

JS:   "ab".repeat(3)
来源：http://hz.316326.xyz/gtjxkvfnps.html

TS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtthdxdqyb.html

Java: "ab".repeat(3)
来源：http://hz.ivvv.top/gtnwilwcfl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gtvxtdjolz.html

Ruby: "ab" * 3
来源：http://hz.haohaochexian.top/gtgzdzgcvf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.quarkkingdee.top/gtoirgwgmt.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtqfpevccx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fengsongda.top/gtrcepaugp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.pycfn.com/gtcdnbtwai.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.shanyushiyangtech.top/gtfwxsqqix.html

TS:   s.slice(1, 4)
来源：http://hz.pycfn.com/gtnctcxndz.html

Java: s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtotartkhe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.fzhhl.top/gtkdtkwhey.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenlongwang.top/gtqzhjzkuj.html

C#:   s.Substring(1, 3)
来源：http://hz.quarkkingdee.top/gtmdaddfgx.html

[E04] 查找子串位置
来源：http://hz.havefunace.top/gtfzsvcavd.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtflrrtjrt.html

PHP:  strpos($s, "x");
来源：http://hz.sweek.top/gtrbvvtvku.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gtqghwwihy.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gtlmtcgctg.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtztczduqr.html

Go:   strings.Index(s, "x")
来源：http://hz.shangyingyoupin.top/gtsjudcdro.html

Ruby: s.index("x")
来源：http://hz.xuanzx.com/gtmcupqvke.html

C#:   s.IndexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtxyefmspv.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.chenjidiqi.icu/gtyablbrgr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fengsongda.top/gtpsykmxjb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ppjwa.cn/gtnzsizqvc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gogol.net.cn/gtnwfkpicm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydjk.org.cn/gtvctetemf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.52xcode.cn/gtnruuvoog.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aibaodan.cn/gtpmsmgzpm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ybcxt.top/gtmrhebnxu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jlsjyb.cn/gtadkqafwq.html


<!-- 参考信息 -->