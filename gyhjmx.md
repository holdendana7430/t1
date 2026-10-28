代发 wailian999

[C14] 泛型函数
来源：http://hz.jiagoushi.top/gtpryoxmbi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.yangfankeji.com/gtydmyjoms.html

PHP:  // 无泛型
来源：http://hz.dianchejie.cn/gttgsaogvt.html

JS:   // 无泛型
来源：http://hz.zhengqikj.top/gtxajocixy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtrcwubgom.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtulzaisrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gogol.net.cn/gteiovddzw.html

Ruby: # 无泛型
来源：http://hz.yj20258.top/gtxgnqaaei.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.sysykeji.top/gtkttdgckf.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtqbqxeizj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhiwuduotai.top/gtadsjbklk.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shangyingyoupin.top/gtzvnksgor.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.birdmap.top/gtqjwxfufs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.c1oappe.top/gtxwkracop.html

Java: // 无解构
来源：http://hz.kuanghao11.cn/gtvkpjobjs.html

Go:   // 无解构
来源：http://hz.jlsjyb.cn/gtnosxpyuu.html

Ruby: a, b = pair
来源：http://hz.dianchejie.cn/gtecidvzgx.html

C#:   var (a, b) = pair;
来源：http://hz.xingfuxueyuan.xyz/gttbzhtqyp.html

[C16] 函数 / 方法重载
来源：http://hz.havefunace.top/gttwblntci.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ywan-chungtsiang.top/gtbdzkgsvb.html

PHP:  // 无重载
来源：http://hz.havefunace.top/gtgcvxvktp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cucudq.cn/gtigpmmrjo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.kuanghao11.cn/gtpugswttz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.wangshuangyany.cn/gtfsrkjaqk.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuanzhike.top/gtcunjhowz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nanxinkj.top/gtbqaramgb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yonumen.top/gthstezzrj.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrghurwoq.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtbfvamqvm.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtwxoexhak.html

[D01] 创建数组 / 列表
来源：http://hz.zhongyouzk.top/gtocoyspnk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.nanxinkj.top/gtqxugwyng.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.snrcjt.cn/gtcufqtbmb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tian-w.cn/gtobigxeso.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pengpengdd.cyou/gttghghqhz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gotoacloud.top/gtlcntqltr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yuanzhike.top/gtsymykndl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhengqikj.top/gtxxnkekyh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sufxvd.cn/gtsdvbhgku.html

[D02] 追加元素到末尾
来源：http://hz.hnxiangtu.top/gtbvtntjit.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sysykeji.top/gturdcpfxv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhengqikj.top/gthrwcpyll.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtegkikpyo.html

TS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtxoznxtww.html

Java: list.add(4);
来源：http://hz.yuxming.cn/gtodhktssf.html

Go:   arr = append(arr, 4)
来源：http://hz.shangyingyoupin.top/gtbnmsohqz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shanyushiyangtech.top/gtwxnvujsb.html

C#:   list.Add(4);
来源：http://hz.redwolf501.top/gtuikxshuw.html

[D03] 在指定位置插入元素
来源：http://hz.9152youxi.cn/gtvcmjlvdr.html

Py:   arr.insert(0, 0)
来源：http://hz.wangshuangyany.cn/gtvbicvwsi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hammf.cn/gteapqgtme.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jyoumei.cn/gtidteikwz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jyoumei.cn/gtoauxnfgt.html

Java: list.add(0, 0);
来源：http://hz.hnxiangtu.top/gtjawuqljf.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ywan-chungtsiang.top/gtncakdmjz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shangyingyoupin.top/gtgkqawncd.html

C#:   list.Insert(0, 0);
来源：http://hz.guowangkeji.top/gtiexbqsrn.html

[D04] 删除元素
来源：http://hz.nwbrower.top/gtadfiugar.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtoduvzpds.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.dianchejie.cn/gtkexckirr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gttjqiphnn.html

TS:   arr.splice(0, 1);
来源：http://hz.yongpay.top/gteuukuydw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hywenlv.cn/gtwnshaphr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ivvv.top/gtrkkqjkud.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gtqzqvyrnj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gtbfmyysrw.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtpkoqbqsi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtnrydyxwj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gtlvbhxbgr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.guowangkeji.top/gtazoazyma.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yueranfly.top/gtzzhsgprz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jinqigufen.top/gtodldmkxp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cashguo.top/gtznzvprvn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtbziqitpz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tanke756.top/gtrbxgvrbi.html

[D06] 数组长度
来源：http://hz.chenjidiqi.icu/gtguzpjcsh.html

Py:   len(arr)
来源：http://hz.gzhubu.top/gtbsfzcdps.html

PHP:  count($arr);
来源：http://hz.wangdashe.top/gtzdzejfnt.html

JS:   arr.length
来源：http://hz.0kj1m.cn/gtqrtcvyac.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gtqnviflqo.html

Java: list.size();
来源：http://hz.tanke756.top/gtdhqnarub.html

Go:   len(arr)
来源：http://hz.jinqigufen.top/gtxzlfcwrm.html

Ruby: arr.length; arr.size
来源：http://hz.kuanghao11.cn/gtdvolophb.html

C#:   list.Count;
来源：http://hz.zhoulong.xyz/gtymmntytn.html

[D07] 切片 / 取子数组
来源：http://hz.ehwqpu.com/gtmzlksjjh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hongshengwenyu.top/gtmftbxlvr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yonumen.top/gtblwiszxs.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtmkhwicqf.html

TS:   arr.slice(1, 4);
来源：http://hz.gogol.net.cn/gtuarkggsb.html

Java: list.subList(1, 4);
来源：http://hz.gaohongyu789.top/gtnztsrqmd.html

Go:   arr[1:4]
来源：http://hz.pengpengdd.cyou/gtkcigfkiw.html

Ruby: arr[1, 3]
来源：http://hz.jinqigufen.top/gtmljrvzmq.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhiwuduotai.top/gtsabyqreh.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gtracvyhra.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgufenzy.top/gtxhynimqp.html

PHP:  array_merge($a, $b);
来源：http://hz.chenzaomai.com/gtfqvoyorr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtmogotguu.html

TS:   [...a, ...b];
来源：http://hz.wangshuangyany.cn/gtyzyobxpd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ywan-chungtsiang.top/gtblevpkda.html

Go:   append(a, b...)
来源：http://hz.yanxiufei.cn/gttpbnrvcz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydjk.org.cn/gtraurkmqs.html

C#:   a.Concat(b).ToList()
来源：http://hz.haohaochexian.top/gtwepuekwr.html

[D09] 排序（升序）
来源：http://hz.yj20258.top/gtjgtlrntq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.bjfxy.top/gtqqmappjx.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gtrmrgwdlo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cdnleiting.top/gtwojclsgt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtefscbxbw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinghuilouyu.cn/gtjzeddswu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xziqi.cn/gtwqcgkimh.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtcpubppsz.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtfyyznvnn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shangyingyoupin.top/gthqfsnrkk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.havefunace.top/gtfxpiueke.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.kuanghao11.cn/gtdxzgczlu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtjilswgnj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtyypynqvj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gogol.net.cn/gtenkwmaqg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gtisiloexi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zhoulong.xyz/gtkiprrzxd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.tanke756.top/gtnjpyolzm.html

[D11] 反转数组
来源：http://hz.svipenyu.cn/gtxoewugbd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yongpay.top/gthbabstuy.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtrtgnyedd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigfzy.top/gtznpjtbhh.html

TS:   [...arr].reverse();
来源：http://hz.quarkkingdee.top/gthqfayojm.html

Java: Collections.reverse(list);
来源：http://hz.yj20258888.top/gtpqtmklym.html

Go:   slices.Reverse(arr)
来源：http://hz.ywan-chungtsiang.top/gtevmodujw.html

Ruby: arr.reverse
来源：http://hz.cucudq.cn/gtpjfcdrcw.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gtahyxghmw.html

[D12] 查找元素下标
来源：http://hz.xuanzx.com/gtebjhgyyt.html

Py:   arr.index(x);  x in arr
来源：http://hz.yonumen.top/gtqgedhunj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.gogol.net.cn/gtdnzzredi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtzzpvpxhf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xylfe.cn/gtjrlqsxgx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jinghuilouyu.cn/gtcbkbnoay.html

Go:   slices.Index(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtvtrdayzn.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gttwdzdhqq.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtmwmtvijz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nanxinkj.top/gtbedvxdtd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtsgexdtlo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtrktkpyjw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtpqqytmhd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtknzxwmop.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.snrcjt.cn/gtajxcdsmu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nwbrower.top/gtsrvfkzjf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ehwqpu.com/gtotmcbare.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.iojbl.cn/gtfimrhbwx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangtech.top/gtcnscmuya.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.316326.xyz/gtlelrcixy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xuetiantiany.cn/gtdznmtjwa.html

JS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtpatrhwjg.html

TS:   arr.map(x => x * 2)
来源：http://hz.jinqigfzy.top/gtpiwgunvz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zycfv.cn/gtrqlizvdz.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtavoomblk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jyoumei.cn/gtkomgsxfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hnxiangtu.top/gtrdvpmnox.html

[D15] 去重
来源：http://hz.xinyue.icu/gtdnezzhpz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj202588.top/gtmwdyvwfx.html

PHP:  array_unique($arr);
来源：http://hz.zdqjudy.top/gtdowtdbzi.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtabqgukzb.html

TS:   [...new Set(arr)]
来源：http://hz.yuanzhike.top/gtsxfuprgv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xylfe.cn/gtwyzpvfip.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangshuangyany.cn/gttvyyoefx.html

Ruby: arr.uniq
来源：http://hz.jianghu66.top/gtraskqxan.html

C#:   list.Distinct().ToList()
来源：http://hz.ehwqpu.com/gtravgdmox.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtvjrwhtcm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.52xcode.cn/gtjuesapbg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.fzhhl.top/gtcmtnbdfv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtmebqhats.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gtoakzdqtu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cheryme.top/gtrdkmakob.html

Go:   // 手写循环累加
来源：http://hz.guowangkeji.top/gtiebuyzxw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtdntmfzcm.html

C#:   list.Sum();  list.Average()
来源：http://hz.sxryk.cn/gtgohdlasv.html

[D17] 最大值与最小值
来源：http://hz.ppjwa.cn/gtxixuyjsu.html

Py:   max(arr);  min(arr)
来源：http://hz.ydzc1.top/gtzxmhcjck.html

PHP:  max($arr);  min($arr);
来源：http://hz.hfpthk.cn/gtxrjlcslv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtnuvhktvg.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangtech.top/gthndrnalh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gttwglrttl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.0kj1m.cn/gtzturwexo.html

Ruby: arr.max;  arr.min
来源：http://hz.jlsjyb.cn/gtugxxnjrd.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtbojdbxxs.html

[D18] 扁平化嵌套数组
来源：http://hz.yangfankeji.com/gtjjzxkbop.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gthhaatiph.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gtotvzafdz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fzhhl.top/gttxioefwy.html

TS:   nested.flat();
来源：http://hz.meibo888.top/gttaperveg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydjk.org.cn/gtcdeaiexq.html

Go:   // 手写双层循环
来源：http://hz.dashuyun.cn/gtaesdlwet.html

Ruby: nested.flatten
来源：http://hz.yongpay.top/gtraqrobvo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nwbrower.top/gtdqqujgmo.html

[D19] 按字段分组
来源：http://hz.yuxming.cn/gtjistqmut.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cheryme.top/gthmnbaplb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tianlin.xyz/gtggfsxqdu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtkqtjtodz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtbffxtuqv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.nanxuanxn.top/gtngrfjetr.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gtmbwqmacr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hnqzz.top/gtcbioyrlt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtfgfujatw.html

[D20] 统计每个元素出现次数
来源：http://hz.daxiang520.top/gtohcmfcax.html

Py:   Counter(arr)
来源：http://hz.gzhubu.top/gttjbwsgnw.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtljmpeqyi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gaohongyu789.top/gtxbyvulry.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtgrvkbnef.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtnpgylyeg.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gtggggswsy.html

Ruby: arr.tally
来源：http://hz.daxiang520.top/gtcepfahgj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jlsjyb.cn/gtfedtksjl.html

[D21] 判断是否包含某元素
来源：http://hz.dashuyun.cn/gtlqiarxgs.html

Py:   x in arr
来源：http://hz.fengsongda.top/gtzrvglsso.html

PHP:  in_array($x, $arr, true);
来源：http://hz.aibaodan.cn/gtwowctgja.html

JS:   arr.includes(x)
来源：http://hz.chenjidiqi.icu/gtbhxegtix.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtvtovplal.html

Java: list.contains(x)
来源：http://hz.snrcjt.cn/gtdfzijnsv.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtxnsrzbts.html

Ruby: arr.include?(x)
来源：http://hz.yonumen.top/gtvdtlpzwr.html

C#:   list.Contains(x)
来源：http://hz.tanke756.top/gtdrfahhya.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cheryme.top/gtcmvrnozr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.aibaodan.cn/gtylogsngl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtqyiqorme.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gttifgwrgv.html

TS:   [...arr];
来源：http://hz.shangyingyoupin.top/gttmoyyhhj.html

Java: new ArrayList<>(list);
来源：http://hz.yvedp.cn/gtkguoqlpz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jiagoushi.top/gtbwizwznu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenjidiqi.icu/gtovvjjgxa.html

C#:   new List<int>(list);
来源：http://hz.hnqzz.top/gtkrtigkek.html

[D23] reduce 累积计算
来源：http://hz.feifeiyinyue.top/gtqsfisqgb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhiwuduotai.top/gtmdiyihly.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.nanxinkj.top/gttrswlsma.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtrsbdvrwh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtrzopsgjd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aibaodan.cn/gtsqhflwlg.html

Go:   // 手写循环
来源：http://hz.jyoumei.cn/gtnjuyiwiy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.52xcode.cn/gtckscuvfb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gaohongyu789.top/gtowfgjywh.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnqzz.top/gtgdgznwav.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ywan-chungtsiang.top/gtekvklkyq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtxrmxnnok.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhixingplan.top/gtoefbklxa.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtbsdufgwt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gtutqqqqog.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.havefunace.top/gtlimurkea.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtmsihupbj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yongpay.top/gtefwtwanx.html

[D25] Set 集合去重与交并差
来源：http://hz.wangshuangyany.cn/gtrybnxzqy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtdnszdviy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgfzy.top/gttnqmnuhi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.pycfn.com/gttibjejga.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hongshengwenyu.top/gtydsdzajd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shzxlz.cn/gtliknjwak.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.svipenyu.cn/gtqbcmyyjc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.52xcode.cn/gtbnjuxrgj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.shangyingyoupin.top/gtevdtcfzx.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtnwdkdbph.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhengqikj.top/gtjcxbmnbb.html

PHP:  implode(", ", $arr);
来源：http://hz.chenzaomai.com/gtvhazvasg.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtlovdtfka.html

TS:   arr.join(", ")
来源：http://hz.pycfn.com/gtbozptwjg.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtdeabntvh.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xingfuxueyuan.xyz/gtgsubrzee.html

Ruby: arr.join(", ")
来源：http://hz.daria6918.cn/gtpesehrfs.html

C#:   string.Join(", ", list)
来源：http://hz.gogol.net.cn/gtqzsjbhgb.html

================================================================================
来源：http://hz.xuanzx.com/gtktxuqhvs.html

E. 字符串处理
来源：http://hz.jinqigufen.top/gtibzfhuif.html

================================================================================
来源：http://hz.ybcxt.top/gtefpangmi.html

[E01] 拼接字符串
来源：http://hz.cheryme.top/gtatuwhmld.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.tian-w.cn/gthwnlyxnp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sysykeji.top/gtxqdbtpvh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtmlenjftj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sysykeji.top/gttrzbvlyg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jinqigfzy.top/gtywehxzad.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenjidiqi.icu/gtsfansuwp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hysaishi.cn/gtjfgkwgcd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.meibo888.top/gtpxgneuzl.html

[E02] 重复字符串
来源：http://hz.wangdashe.top/gtaqtyikfo.html

Py:   "ab" * 3
来源：http://hz.yanxiufei.cn/gtvtgvuibi.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtomhbpddr.html

JS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtecnwfobx.html

TS:   "ab".repeat(3)
来源：http://hz.yvedp.cn/gtwsfqalov.html

Java: "ab".repeat(3)
来源：http://hz.zhongyouzk.top/gttylqfens.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ppjwa.cn/gtouaticvr.html

Ruby: "ab" * 3
来源：http://hz.hammf.cn/gtfpcldunk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.redwolf501.top/gtifjjobnw.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtydnsiyhr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fzhhl.top/gtfyuihwud.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhoulong.xyz/gtqpcrzkjd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.xinyue.icu/gtopjijjmd.html

TS:   s.slice(1, 4)
来源：http://hz.zdqjudy.top/gtbidtfeov.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gttnzbybub.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.smart0.xyz/gtwhfnwiol.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hywenlv.cn/gtgsxoxzjt.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigufen.top/gteitdagzn.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtnmiusnaa.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtnmktjxod.html

PHP:  strpos($s, "x");
来源：http://hz.gaohongyu789.top/gtnriwcbzl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xuetiantiany.cn/gtotuktfmt.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtalpejokl.html

Java: s.indexOf("x")
来源：http://hz.smart0.xyz/gtglbedejp.html


<!-- 参考信息 -->