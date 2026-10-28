代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.fzhhl.top/gtiznunnge.html

[C15] 解构 / 展开参数
来源：http://hz.sufxvd.cn/gtoyqvxorv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gtjuznvrur.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sxryk.cn/gtojeiwzjf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258.top/gtrkmulgpd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.tanke756.top/gtvekounog.html

Java: // 无解构
来源：http://hz.jiagoushi.top/gtxttgtqfs.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gteqhzsrqn.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtllgpcleq.html

C#:   var (a, b) = pair;
来源：http://hz.dianchejie.cn/gtylvkmnsn.html

[C16] 函数 / 方法重载
来源：http://hz.daxiang520.top/gtavymhwgg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pengpengdd.cyou/gtoolembpc.html

PHP:  // 无重载
来源：http://hz.cdnleiting.top/gtajyboxyj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinghuilouyu.cn/gtallwjhcd.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yonumen.top/gtaokofjgd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtcqthnpao.html

Go:   // 无重载：用不同函数名
来源：http://hz.dianchejie.cn/gtztbwstht.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ppjwa.cn/gtzgaafrjj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangdashe.top/gtreygqvyt.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtchytyhkm.html

D. 数组 / 列表 / 集合
来源：http://hz.yangfankeji.com/gthzadkpwi.html

================================================================================
来源：http://hz.zhijiandao.cn/gthknoqgwa.html

[D01] 创建数组 / 列表
来源：http://hz.sxryk.cn/gtjwwckocr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.svipenyu.cn/gtiqlrhjfl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yangfankeji.com/gtbqiolphk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.vqdsnc.cn/gtypgbdxwv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xingfuxueyuan.xyz/gtwdxwkvrv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cdnleiting.top/gtmwfzvbva.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.andypj.xyz/gtkmbbadvh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuanzhike.top/gtjhohjlwg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yj202588.top/gtdbrxxekk.html

[D02] 追加元素到末尾
来源：http://hz.ydjk.org.cn/gteozlbfwq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yanxiufei.cn/gtzekgegmw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangdashe.top/gtzpcvygfq.html

JS:   arr.push(4);
来源：http://hz.yonumen.top/gthxfthffm.html

TS:   arr.push(4);
来源：http://hz.hongshengwenyu.top/gtzqwvsmrh.html

Java: list.add(4);
来源：http://hz.nanxinkj.top/gtdtevvsiv.html

Go:   arr = append(arr, 4)
来源：http://hz.aibaodan.cn/gtilitricg.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtyntmttck.html

C#:   list.Add(4);
来源：http://hz.gzhubu.top/gtraxihtht.html

[D03] 在指定位置插入元素
来源：http://hz.shanyushiyangkeji.top/gtyhdjldzb.html

Py:   arr.insert(0, 0)
来源：http://hz.feifeiyinyue.top/gttztiaema.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtnkpuouhj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.chenjidiqi.icu/gthmugdjfk.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.gzhubu.top/gtfinjtkoe.html

Java: list.add(0, 0);
来源：http://hz.redwolf501.top/gtfkrviwfw.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.cdnleiting.top/gtxfisflsf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gogol.net.cn/gtampkouas.html

C#:   list.Insert(0, 0);
来源：http://hz.9152youxi.cn/gtwhtoktbd.html

[D04] 删除元素
来源：http://hz.zhaomingkeji.xyz/gtcmfefqlu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fzhhl.top/gtthjocxvi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinghuilouyu.cn/gtveqbmraz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gtsishrnuu.html

TS:   arr.splice(0, 1);
来源：http://hz.bjfxy.top/gtyrreqokl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.havefunace.top/gteqiprveq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.xuanzx.com/gtsnvwgdip.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shzxlz.cn/gtnqnmpxnn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.c1oappe.top/gttlrhhdds.html

[D05] 访问与修改元素
来源：http://hz.pycfn.com/gtksyunloz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.bjfxy.top/gtzctaexwm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zdqjudy.top/gtvimchtwy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.9152youxi.cn/gtzbdsuczy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.c1oappe.top/gtjmpwzwac.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yueranfly.top/gtbmhtthpo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yueranfly.top/gtzxxojhkv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtholsltxu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ehwqpu.com/gteekuaktk.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gthzwwtkjy.html

Py:   len(arr)
来源：http://hz.fengsongda.top/gtfdcfpoic.html

PHP:  count($arr);
来源：http://hz.jinqigufen.top/gtjuiamnwy.html

JS:   arr.length
来源：http://hz.nanxuanxn.top/gtqummtcsh.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gtxfyjjjal.html

Java: list.size();
来源：http://hz.zdqjudy.top/gtnnrjgbsl.html

Go:   len(arr)
来源：http://hz.yanxiufei.cn/gteqiturye.html

Ruby: arr.length; arr.size
来源：http://hz.kuanghao11.cn/gthgofdmhb.html

C#:   list.Count;
来源：http://hz.ehwqpu.com/gtyscghwrl.html

[D07] 切片 / 取子数组
来源：http://hz.guannengcc.top/gtwaakdqus.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuetiantiany.cn/gtbtseuini.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.snrcjt.cn/gtoppwkouf.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtwznxaocb.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtjjypnrnx.html

Java: list.subList(1, 4);
来源：http://hz.jinqigufen.top/gtppxgncjv.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtasfardoh.html

Ruby: arr[1, 3]
来源：http://hz.shanyushiyangkeji.top/gtlhqewefm.html

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtqbdnpsms.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangkeji.top/gtqfvhocuu.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtwuzslxed.html

PHP:  array_merge($a, $b);
来源：http://hz.sysykeji.top/gtxsxozjhk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ywan-chungtsiang.top/gtgvrpcips.html

TS:   [...a, ...b];
来源：http://hz.ivvv.top/gtdeecvdaj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.quarkkingdee.top/gtusxyictb.html

Go:   append(a, b...)
来源：http://hz.nwbrower.top/gtaisdltrr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yueranfly.top/gtilibyjbr.html

C#:   a.Concat(b).ToList()
来源：http://hz.daxiang520.top/gtlnyygzsb.html

[D09] 排序（升序）
来源：http://hz.tianlin.xyz/gtqfhlkcjd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtiuhgbhwg.html

PHP:  sort($arr);
来源：http://hz.quarkkingdee.top/gteaxpbnyw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jyoumei.cn/gtiynahubv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtndbpdxth.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.bjfxy.top/gtyxxjtyft.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ehwqpu.com/gtelzlauzk.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtthbvgdtu.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtvikjgbsd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hfpthk.cn/gtvdlyappi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtrjqxlakk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtfzvzqvkp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtekpbzjan.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtatmaoqti.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ehwqpu.com/gtqveropdq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.tianlin.xyz/gtqlrfzpzm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tanke756.top/gtugnqutvi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gttzssrkdn.html

[D11] 反转数组
来源：http://hz.hnxiangtu.top/gtkodzbmld.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangshuangyany.cn/gtfevmrktq.html

PHP:  array_reverse($arr);
来源：http://hz.shangyingyoupin.top/gtoqxayble.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hfpthk.cn/gtibxqcqyk.html

TS:   [...arr].reverse();
来源：http://hz.haohaochexian.top/gtoeynkrzp.html

Java: Collections.reverse(list);
来源：http://hz.9152youxi.cn/gtmfpfpudr.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtbsjpokig.html

Ruby: arr.reverse
来源：http://hz.chenzaomai.com/gteqkkwgux.html

C#:   list.Reverse();
来源：http://hz.yvedp.cn/gtlpwkjuhb.html

[D12] 查找元素下标
来源：http://hz.hfpthk.cn/gtdkeqshty.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhixingplan.top/gtkshtdggw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhiwuduotai.top/gtknjlgwat.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gthykrbkpg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtpdkpwpnk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtjobzafrt.html

Go:   slices.Index(arr, x)
来源：http://hz.iojbl.cn/gtsbssmcaj.html

Ruby: arr.index(x)
来源：http://hz.shzxlz.cn/gtwnhetakm.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gtnbmgpvol.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtrvkyobtn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gtntijpfqb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tianlin.xyz/gtrahlevup.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtizdxtjws.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nwbrower.top/gtgobzxouj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cucudq.cn/gtiktfurfv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yueranfly.top/gtozhbdrpe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gogol.net.cn/gtkwutfspg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtqhifsbqn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangdashe.top/gtgfpkxalw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuanzhike.top/gtaqueuplj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtsddbkzja.html

JS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gthxyrfwqk.html

TS:   arr.map(x => x * 2)
来源：http://hz.daria6918.cn/gtjnfhulua.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gtpqhfmmvn.html

Go:   // 手写循环
来源：http://hz.cqqwz.cn/gtugottoti.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtykhqqdjo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gotoacloud.top/gtoeyggyso.html

[D15] 去重
来源：http://hz.xziqi.cn/gtlyzmyvgc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xuanzx.com/gtiuckgclt.html

PHP:  array_unique($arr);
来源：http://hz.hysaishi.cn/gtujohuxeq.html

JS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtugfgmmrr.html

TS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtrpxhdtox.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.svipenyu.cn/gtuwfdghai.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yvedp.cn/gtssqreiof.html

Ruby: arr.uniq
来源：http://hz.cdnleiting.top/gtvmwpfwkm.html

C#:   list.Distinct().ToList()
来源：http://hz.jlsjyb.cn/gttabqelbx.html

[D16] 求和与平均值
来源：http://hz.fengsongda.top/gtkqwcsovd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtlsmodrly.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.andypj.xyz/gtygmdtuuh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtgdxlbsjg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xylfe.cn/gtqweqyyfs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sweek.top/gtjwiyqjte.html

Go:   // 手写循环累加
来源：http://hz.0kj1m.cn/gtkbpxceje.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtcqaepfiy.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gtedbequwk.html

[D17] 最大值与最小值
来源：http://hz.chenjidiqi.icu/gtzfwgddin.html

Py:   max(arr);  min(arr)
来源：http://hz.tanke756.top/gtudwenrjc.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtgtifziyu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tanke756.top/gtyqkggaeq.html

TS:   Math.max(...arr);
来源：http://hz.yj20258888.top/gtpdklmckf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pycfn.com/gtlrfczlfu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtmfzdefgk.html

Ruby: arr.max;  arr.min
来源：http://hz.chenjidiqi.icu/gtddjosolf.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtygxzfprp.html

[D18] 扁平化嵌套数组
来源：http://hz.aizwys.cn/gtqwvkikmx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xziqi.cn/gtoshmaafo.html

PHP:  array_merge(...$nested);
来源：http://hz.tanke756.top/gtbdxljgdm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shanyushiyangkeji.top/gtskrlmzbf.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtguosupnd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtitvnhevv.html

Go:   // 手写双层循环
来源：http://hz.jyoumei.cn/gtszfpdukp.html

Ruby: nested.flatten
来源：http://hz.sysykeji.top/gtqalniszr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gtsqvwxpqz.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtrwgtixtw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.guowangkeji.top/gthfmtisqd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.0kj1m.cn/gtfbxyktva.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenzaomai.com/gtnchoyvgw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtspqhtogy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yuanzhike.top/gtvilpvcjv.html

Go:   // 手写 map[string][]T
来源：http://hz.wangdashe.top/gtiisqicih.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtzyiccbjf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hammf.cn/gtjfusnzly.html

[D20] 统计每个元素出现次数
来源：http://hz.jiagoushi.top/gthhuuhyvx.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtjyigxxpy.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gtdszwelns.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtzdbgoeor.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtczeiaknz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.birdmap.top/gtmvzajkos.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtkhxbzoyc.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtqalvacna.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhengqikj.top/gtqvveycxb.html

[D21] 判断是否包含某元素
来源：http://hz.pengpengdd.cyou/gtrmctsrfp.html

Py:   x in arr
来源：http://hz.bjfxy.top/gtwrjiaafc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.shanyushiyangkeji.top/gtzoaeqhmy.html

JS:   arr.includes(x)
来源：http://hz.dianchejie.cn/gteclflnis.html

TS:   arr.includes(x)
来源：http://hz.shangyingyoupin.top/gtwaquavgy.html

Java: list.contains(x)
来源：http://hz.hammf.cn/gtgwhiqocc.html

Go:   slices.Contains(arr, x)
来源：http://hz.dashuyun.cn/gtzzjhbkxt.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gtubrcssqi.html

C#:   list.Contains(x)
来源：http://hz.zdqjudy.top/gtvpevjhds.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yonumen.top/gthfijqocy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jqgfzy.top/gtingyznia.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.xinyue.icu/gtbritudcm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.aibaodan.cn/gtxnfbtoih.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtuzgvmfdm.html

Java: new ArrayList<>(list);
来源：http://hz.gzhubu.top/gtaoaxvjjy.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.birdmap.top/gtlubhptqk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtvgnmtxsn.html

C#:   new List<int>(list);
来源：http://hz.9152youxi.cn/gtbbqeskfs.html

[D23] reduce 累积计算
来源：http://hz.guowangkeji.top/gtewgwcrgs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.sxryk.cn/gtyasxsbgh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.havefunace.top/gtlqlmzymq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.316326.xyz/gtqbzdsozp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nwbrower.top/gtulciakih.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.bjfxy.top/gtlqpxllsy.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtqfoqimle.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gtlextamob.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtoytnfxdh.html

[D24] 字典 / Map 基本操作
来源：http://hz.sufxvd.cn/gtthiihlxf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtwnevuwmp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.52xcode.cn/gtuqpzpmhx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xinyue.icu/gtgftiufes.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtwotuyrzk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.birdmap.top/gtqiokxoxb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ppjwa.cn/gtlxklsfrv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gogol.net.cn/gttffojfdk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtmtyfjnvk.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gthhcbzcra.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtsrnkzdnq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtqamehmpp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtcdlxufxw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenzaomai.com/gtbdngnkbp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gotoacloud.top/gtqzobiyrl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtuzbeeuna.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgufenzy.top/gtureqwbwm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cqqwz.cn/gtosqgqtxa.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtvkimzmfd.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gthmmhnsol.html

PHP:  implode(", ", $arr);
来源：http://hz.daria6918.cn/gttueluaub.html

JS:   arr.join(", ")
来源：http://hz.cdnleiting.top/gtbtixlhrp.html

TS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtolruhysv.html

Java: String.join(", ", list)
来源：http://hz.quarkkingdee.top/gtjsiwdhqw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ywan-chungtsiang.top/gthooirvaz.html

Ruby: arr.join(", ")
来源：http://hz.hammf.cn/gthpkwexaa.html

C#:   string.Join(", ", list)
来源：http://hz.jiagoushi.top/gtkwjwrpol.html

================================================================================
来源：http://hz.daria6918.cn/gtumoihhgj.html

E. 字符串处理
来源：http://hz.jinyuanbaomall.cn/gtzzpmnmek.html

================================================================================
来源：http://hz.9152youxi.cn/gthtikvqam.html

[E01] 拼接字符串
来源：http://hz.bjfxy.top/gtobsembnu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.daxiang520.top/gtueqmywch.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.meibo888.top/gtmactozjw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtzttyfugo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ppjwa.cn/gtfaeyosmo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hysaishi.cn/gteqczpplq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangtech.top/gtcxutugdp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fengsongda.top/gtmrizyhap.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtpnevtwrp.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtweynghah.html

Py:   "ab" * 3
来源：http://hz.zdqjudy.top/gtsyvcxvll.html

PHP:  str_repeat("ab", 3);
来源：http://hz.0kj1m.cn/gtvylitzog.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtuxjjovzh.html

TS:   "ab".repeat(3)
来源：http://hz.yangfankeji.com/gtltsbclpr.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtcsggrpwm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.guannengcc.top/gtpflwjalm.html

Ruby: "ab" * 3
来源：http://hz.quarkkingdee.top/gtdyglpqfu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gtmnlispbf.html

[E03] 截取子串
来源：http://hz.meibo888.top/gthpabrysk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.gogol.net.cn/gtemnxnnxw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jinqigfzy.top/gtxpnwhibt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gogol.net.cn/gttruarxua.html

TS:   s.slice(1, 4)
来源：http://hz.yuanzhike.top/gtzkszdsvs.html

Java: s.substring(1, 4)
来源：http://hz.redwolf501.top/gtenooegys.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydjk.org.cn/gttjbzsxkc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuxming.cn/gtaxitxgkv.html

C#:   s.Substring(1, 3)
来源：http://hz.jqgfzy.top/gtadkozugk.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtyptxzegq.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fzhhl.top/gteongqvzb.html

PHP:  strpos($s, "x");
来源：http://hz.hnxiangtu.top/gthhvrklsx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jinqigufen.top/gtartrioxw.html

TS:   s.indexOf("x")
来源：http://hz.tanke756.top/gthoreastf.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtgsrnykrw.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtasrvfflg.html

Ruby: s.index("x")
来源：http://hz.sxryk.cn/gthdjimhtg.html

C#:   s.IndexOf("x")
来源：http://hz.pengpengdd.cyou/gtccandhci.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shuidangran.top/gtqxlkyvhf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.chenjidiqi.icu/gtlmeswhjm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhijiandao.cn/gteverhmsz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yonumen.top/gtmuexeokr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ybcxt.top/gtymbpokyk.html


<!-- 参考信息 -->