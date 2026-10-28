代发 wailian999

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.smart0.xyz/gteuozvydm.html

[C15] 解构 / 展开参数
来源：http://hz.c1oappe.top/gtvbdtjuuw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtqtvbfugf.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gaohongyu789.top/gtllmazrma.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtldeqdjjw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhixingplan.top/gtougqmraa.html

Java: // 无解构
来源：http://hz.hnxiangtu.top/gtxhmrtbae.html

Go:   // 无解构
来源：http://hz.sxryk.cn/gtnidsmogj.html

Ruby: a, b = pair
来源：http://hz.jinqigfzy.top/gtekckheem.html

C#:   var (a, b) = pair;
来源：http://hz.mhx1999.top/gtgpdrmauc.html

[C16] 函数 / 方法重载
来源：http://hz.snrcjt.cn/gtkcdvtsph.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtvfflthaq.html

PHP:  // 无重载
来源：http://hz.yangfankeji.com/gtmyrvxilf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigufen.top/gtmzrwemkl.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nwbrower.top/gtbnbbiidg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgufenzy.top/gtmfcawpqx.html

Go:   // 无重载：用不同函数名
来源：http://hz.aibaodan.cn/gtwcefuprn.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tianlin.xyz/gtdresmbtz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yongpay.top/gthiqrkqny.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdeszdedm.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgfzy.top/gtpaahyhtx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtuwibwkrm.html

[D01] 创建数组 / 列表
来源：http://hz.havefunace.top/gttpxqdbmm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj202588.top/gtmvfrtsoc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigfzy.top/gtclawjtkk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jianghu66.top/gtzhnrmsuk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.wangshuangyany.cn/gtvfxuxbhk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj20258.top/gthlqmcnim.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.mhx1999.top/gtfntwxbvn.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xylfe.cn/gtxjogatrr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ppjwa.cn/gtgrbpuqsu.html

[D02] 追加元素到末尾
来源：http://hz.jinqigfzy.top/gtpoqgcndb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenzaomai.com/gtbicrotpi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yanxiufei.cn/gtlbsxggso.html

JS:   arr.push(4);
来源：http://hz.ppjwa.cn/gtnarilimh.html

TS:   arr.push(4);
来源：http://hz.shangyingyoupin.top/gtriokhifc.html

Java: list.add(4);
来源：http://hz.c1oappe.top/gtpmaiicrw.html

Go:   arr = append(arr, 4)
来源：http://hz.xinyue.icu/gtcwrssvmc.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuxming.cn/gtxaxfkytd.html

C#:   list.Add(4);
来源：http://hz.shangyingyoupin.top/gtklypiffg.html

[D03] 在指定位置插入元素
来源：http://hz.nanxuanxn.top/gtfdctgmwj.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtrwvcjjdy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.redwolf501.top/gtlarvpfgf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.c1oappe.top/gtujxbrvuu.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtmyjmqgsy.html

Java: list.add(0, 0);
来源：http://hz.tanke756.top/gtgmwjvewl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258888.top/gtzyzogyeu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258888.top/gtzdjawllu.html

C#:   list.Insert(0, 0);
来源：http://hz.cheryme.top/gtgovzyrtp.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtzbtqfulg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtblarwgin.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtuqfyfgef.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cucudq.cn/gtbpwgveme.html

TS:   arr.splice(0, 1);
来源：http://hz.jinyuanbaomall.cn/gtdhulqfdl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtcqjpvtni.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jqgufenzy.top/gtdhmrgiit.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.birdmap.top/gtnopzjpmi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gtzfmqpyvc.html

[D05] 访问与修改元素
来源：http://hz.xinyue.icu/gtdbvpqdcp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtyjbtuxmp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.c1oappe.top/gtwzvzimxx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhaomingkeji.xyz/gthczxidpw.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gttnxvzuxx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.xuanzx.com/gtqkndqofa.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sufxvd.cn/gtzisxshou.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtvrxdhuro.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgfzy.top/gtlikbbhtg.html

[D06] 数组长度
来源：http://hz.zdqjudy.top/gtivbjonxx.html

Py:   len(arr)
来源：http://hz.jqgufenzy.top/gtmmagcsef.html

PHP:  count($arr);
来源：http://hz.yueranfly.top/gtrcafismj.html

JS:   arr.length
来源：http://hz.sweek.top/gtkdwipdyr.html

TS:   arr.length
来源：http://hz.chenjidiqi.icu/gtxrszdgqw.html

Java: list.size();
来源：http://hz.yj20258888.top/gtbblazlut.html

Go:   len(arr)
来源：http://hz.yueranfly.top/gtkhbxihql.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gtrwmvlvrn.html

C#:   list.Count;
来源：http://hz.haohaochexian.top/gtjlkbzpwd.html

[D07] 切片 / 取子数组
来源：http://hz.fengsongda.top/gtjzfelqbz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yonumen.top/gtcqaniqyp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jiagoushi.top/gtrsnhvmrj.html

JS:   arr.slice(1, 4);
来源：http://hz.tian-w.cn/gtxllnlgky.html

TS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtwskdpnme.html

Java: list.subList(1, 4);
来源：http://hz.daria6918.cn/gtqiqaqllv.html

Go:   arr[1:4]
来源：http://hz.pycfn.com/gtwwpnhofn.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtekyttxru.html

C#:   list.GetRange(1, 3);
来源：http://hz.snrcjt.cn/gtmnnlhikx.html

[D08] 合并两个数组
来源：http://hz.gotoacloud.top/gtkxmrswxs.html

Py:   a + b;  a.extend(b)
来源：http://hz.tanke756.top/gtnchcsfzk.html

PHP:  array_merge($a, $b);
来源：http://hz.jlsjyb.cn/gtyaozoogh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jyoumei.cn/gtxnhmieis.html

TS:   [...a, ...b];
来源：http://hz.316326.xyz/gtzhgfsxbs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtvakucbmt.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gthcgetfpu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gthoibvuaj.html

C#:   a.Concat(b).ToList()
来源：http://hz.sxryk.cn/gtqzleglrx.html

[D09] 排序（升序）
来源：http://hz.sysykeji.top/gtxunfnubk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtlytbchff.html

PHP:  sort($arr);
来源：http://hz.52xcode.cn/gtqvakaxga.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenjidiqi.icu/gtbwwxnlxo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtqzegmxvq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydjk.org.cn/gtbobaazdv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sxryk.cn/gtaggyrmmo.html

Ruby: arr.sort
来源：http://hz.yvedp.cn/gtcaqpkolr.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gtpwoypnxv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtawgkrjad.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtoqowwhqt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.snrcjt.cn/gtyrzcqepn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtmsloghcr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtukibfyzr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtnybemkms.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gttthgurjy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.iojbl.cn/gtgydjcmdd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhongyouzk.top/gtvarnutlp.html

[D11] 反转数组
来源：http://hz.gogol.net.cn/gtuyeevsun.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cashguo.top/gtpvmytfxs.html

PHP:  array_reverse($arr);
来源：http://hz.jinyuanbaomall.cn/gtoknjpsqr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gteipkvetd.html

TS:   [...arr].reverse();
来源：http://hz.hammf.cn/gtnpspwbzc.html

Java: Collections.reverse(list);
来源：http://hz.xylfe.cn/gtbkbqatap.html

Go:   slices.Reverse(arr)
来源：http://hz.ppjwa.cn/gtqhvjbucq.html

Ruby: arr.reverse
来源：http://hz.daria6918.cn/gtgkabjzbr.html

C#:   list.Reverse();
来源：http://hz.sysykeji.top/gtbtqjmjgd.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtpnlhtgid.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuetiantiany.cn/gtzgqcgxxe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtpxtfxyfh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtlhamliqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtzlsrdtrj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gttusrnlqx.html

Go:   slices.Index(arr, x)
来源：http://hz.mhx1999.top/gtklohbzpp.html

Ruby: arr.index(x)
来源：http://hz.xinyue.icu/gtohegeqjd.html

C#:   list.IndexOf(x);
来源：http://hz.yonumen.top/gtinyvkvha.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenzaomai.com/gtzbtzivna.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gzhubu.top/gtddhgyntm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.tian-w.cn/gttohgnhaf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.havefunace.top/gthgnqpurm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtirpujlhh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hammf.cn/gtkirljjbq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.vqdsnc.cn/gtxrxepequ.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.mhx1999.top/gtaqffzald.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.wangdashe.top/gtwuptqhka.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtfivjsnjw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenjidiqi.icu/gtnilvmknu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hammf.cn/gtwxhuvbwn.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxinkj.top/gtsrxbefox.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gthndidhko.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yanxiufei.cn/gtodvswazg.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtgefycqeb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jqgufenzy.top/gtzyyxdglp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtinighkru.html

[D15] 去重
来源：http://hz.cheryme.top/gtzcfskvcm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shuidangran.top/gtrtdtmsrq.html

PHP:  array_unique($arr);
来源：http://hz.zhengqikj.top/gtpabrxegg.html

JS:   [...new Set(arr)]
来源：http://hz.xingfuxueyuan.xyz/gtxjidesre.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtujryzlnh.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtvjdvelns.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenjidiqi.icu/gtucevbplt.html

Ruby: arr.uniq
来源：http://hz.gaohongyu789.top/gtpfdfamsp.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtfqsrcuud.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gttfyftdgt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.fengsongda.top/gtcusrqzpq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.svipenyu.cn/gtdwrzfzqg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtwqnmolmc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtexkkmauw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtucxbqfyf.html

Go:   // 手写循环累加
来源：http://hz.iojbl.cn/gthdhdwrgz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xingfuxueyuan.xyz/gtygmcexge.html

C#:   list.Sum();  list.Average()
来源：http://hz.tanke756.top/gtljqipxqs.html

[D17] 最大值与最小值
来源：http://hz.jianghu66.top/gtvqqreahg.html

Py:   max(arr);  min(arr)
来源：http://hz.zdqjudy.top/gtvuqiaoxr.html

PHP:  max($arr);  min($arr);
来源：http://hz.tanke756.top/gtyybsfzek.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtsfbobpoy.html

TS:   Math.max(...arr);
来源：http://hz.quarkkingdee.top/gtvoccfebk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yj20258.top/gthxfxmhmq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fzhhl.top/gttxdqgbvd.html

Ruby: arr.max;  arr.min
来源：http://hz.ppjwa.cn/gttgrjcrgr.html

C#:   list.Max();  list.Min()
来源：http://hz.yangfankeji.com/gtqwdlkhgi.html

[D18] 扁平化嵌套数组
来源：http://hz.xziqi.cn/gtkpyipsfs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.smart0.xyz/gtjekzllvf.html

PHP:  array_merge(...$nested);
来源：http://hz.9152youxi.cn/gtypqwdjtc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ywan-chungtsiang.top/gtomcxclcl.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtniegthac.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.316326.xyz/gthqmszbdk.html

Go:   // 手写双层循环
来源：http://hz.cqqwz.cn/gtipjgkdoq.html

Ruby: nested.flatten
来源：http://hz.gogol.net.cn/gtxbyijmrl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtkcskothd.html

[D19] 按字段分组
来源：http://hz.hfpthk.cn/gtcvwgosma.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.andypj.xyz/gtmqjpwzhg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtyczulhcm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tianlin.xyz/gtgpgoutcd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yonumen.top/gtbiwnvgkg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.chenlongwang.top/gtxrzdzjgi.html

Go:   // 手写 map[string][]T
来源：http://hz.feifeiyinyue.top/gtvhoyfyox.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhengqikj.top/gtnyolbzaj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jqgfzy.top/gtxwhmycoi.html

[D20] 统计每个元素出现次数
来源：http://hz.zhongyouzk.top/gtswgebfux.html

Py:   Counter(arr)
来源：http://hz.zhengqikj.top/gtspdxhvyq.html

PHP:  array_count_values($arr);
来源：http://hz.ydjk.org.cn/gtrmwcybjw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtjuqiucrv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ehwqpu.com/gtawmlzrba.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xuanzx.com/gtqbieydpa.html

Go:   // 手写 map[T]int
来源：http://hz.316326.xyz/gtibwygugg.html

Ruby: arr.tally
来源：http://hz.svipenyu.cn/gtbkntcarw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yongpay.top/gtfdorqxjo.html

[D21] 判断是否包含某元素
来源：http://hz.jianghu66.top/gtcsdpnpil.html

Py:   x in arr
来源：http://hz.zhengqikj.top/gtsehejiid.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtvwnbiaya.html

JS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtlswzylpq.html

TS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtxqnbblwi.html

Java: list.contains(x)
来源：http://hz.gaohongyu789.top/gtgnfuayfn.html

Go:   slices.Contains(arr, x)
来源：http://hz.tianlin.xyz/gtbtidkjob.html

Ruby: arr.include?(x)
来源：http://hz.ppjwa.cn/gtcgocjyci.html

C#:   list.Contains(x)
来源：http://hz.yuanzhike.top/gtfdwenhrs.html

[D22] 复制数组（避免共享引用）
来源：http://hz.c1oappe.top/gtkuaufkto.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenlongwang.top/gtiowoyazq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtsqppvbde.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhixingplan.top/gtqfasndja.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtlpjilayq.html

Java: new ArrayList<>(list);
来源：http://hz.gogol.net.cn/gtohidtdrn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xuanzx.com/gtpmsubwjs.html

Ruby: arr.dup;  arr.clone
来源：http://hz.tanke756.top/gtgoyeenpq.html

C#:   new List<int>(list);
来源：http://hz.jinyuanbaomall.cn/gtwpdknuhm.html

[D23] reduce 累积计算
来源：http://hz.cheryme.top/gtpefmekld.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ybcxt.top/gtlgtrywmx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cucudq.cn/gtczddrrks.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tian-w.cn/gtqnsyswik.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtgatoyaub.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gogol.net.cn/gtpfdogovv.html

Go:   // 手写循环
来源：http://hz.yj20258.top/gtgkijepkj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhongyouzk.top/gtlzyyzzog.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daria6918.cn/gtlfrxfccz.html

[D24] 字典 / Map 基本操作
来源：http://hz.svipenyu.cn/gtpgjvroki.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jlsjyb.cn/gtgrpmbaux.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yonumen.top/gttzreghbn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtnlnrvvdr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhixingplan.top/gthfiivthc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sufxvd.cn/gtexrktear.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.snrcjt.cn/gtprfdllwj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtogdzaxuo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.dashuyun.cn/gtffrxwupf.html

[D25] Set 集合去重与交并差
来源：http://hz.iojbl.cn/gtwgepvmuw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yangfankeji.com/gtkehwnzro.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.mhx1999.top/gtucjmpkol.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhaomingkeji.xyz/gtsyvwginv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghu66.top/gtkuhetmgh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gaohongyu789.top/gtmyumrsub.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gthnhoualt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gzhubu.top/gtblxkiive.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtklotiutw.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtcpydzarp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtfdopgdng.html

PHP:  implode(", ", $arr);
来源：http://hz.yueranfly.top/gtulnmeceq.html

JS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtaxwudqpa.html

TS:   arr.join(", ")
来源：http://hz.yj202588.top/gtkuuthgva.html

Java: String.join(", ", list)
来源：http://hz.ywan-chungtsiang.top/gtmblzmumy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cdnleiting.top/gtztzembnf.html

Ruby: arr.join(", ")
来源：http://hz.yj20258.top/gtqsawpzpm.html

C#:   string.Join(", ", list)
来源：http://hz.nanxuanxn.top/gtsyqtcqfv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtuqmnfeot.html

E. 字符串处理
来源：http://hz.quarkkingdee.top/gtkqnbgumc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtphumznvq.html

[E01] 拼接字符串
来源：http://hz.fengsongda.top/gtnvozqmqc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shzxlz.cn/gtmcpwpysw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.sweek.top/gtikerhjdd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gttxouqosl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj20258.top/gtpkcbbdjo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.mhx1999.top/gtclgfvbmp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.tianlin.xyz/gtmlnaybsw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xingfuxueyuan.xyz/gtxsnyyrhy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenlongwang.top/gtawkkcbcl.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gtkxdlvdxr.html

Py:   "ab" * 3
来源：http://hz.daxiang520.top/gtdgpdmuyt.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenzaomai.com/gtwxipcbve.html

JS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtxedwaqgh.html

TS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtqsihgqlv.html

Java: "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtretrqowm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.mhx1999.top/gtlathmjdd.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtlyvxfuri.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgfzy.top/gtrpmjeyns.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gttmypbpgv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtekmekfkl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtpwedeaxv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ydzc1.top/gtnthrwyca.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtuyakdohs.html

Java: s.substring(1, 4)
来源：http://hz.ybcxt.top/gtmzgitwdy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guowangkeji.top/gtovjrwdgh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtyvrarzvz.html

C#:   s.Substring(1, 3)
来源：http://hz.zhengqikj.top/gtpcjateyo.html

[E04] 查找子串位置
来源：http://hz.guannengcc.top/gtcfztaesu.html

Py:   s.find("x");  s.index("x")
来源：http://hz.sufxvd.cn/gtzjvjyjff.html

PHP:  strpos($s, "x");
来源：http://hz.yonumen.top/gtyzhbrrdc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgfzy.top/gtjcqlntot.html

TS:   s.indexOf("x")
来源：http://hz.meibo888.top/gttgcqfdif.html

Java: s.indexOf("x")
来源：http://hz.yueranfly.top/gtoboigeha.html

Go:   strings.Index(s, "x")
来源：http://hz.haohaochexian.top/gtyfzrbiyy.html

Ruby: s.index("x")
来源：http://hz.meibo888.top/gtodhhlfzo.html

C#:   s.IndexOf("x")
来源：http://hz.cheryme.top/gtnulzpbsq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zdqjudy.top/gtnzrmduqu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.tanke756.top/gtomardmsr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shanyushiyangkeji.top/gtxlggdikz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtuxfrvity.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.jinqigfzy.top/gtbrxywejg.html


<!-- 参考信息 -->