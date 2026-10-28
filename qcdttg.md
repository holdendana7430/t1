代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hfpthk.cn/gtvbgrxdmo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.bjfxy.top/gtctwabupb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shangyingyoupin.top/gtapipbrba.html

Ruby: # 无泛型
来源：http://hz.ywan-chungtsiang.top/gttwkxxmqa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shanyushiyangkeji.top/gtxmoicmun.html

[C15] 解构 / 展开参数
来源：http://hz.fengsongda.top/gtabtxtxjs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.snrcjt.cn/gtyhmdxvxt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sufxvd.cn/gtqnttksld.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtebowvero.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.havefunace.top/gtrwfxzxet.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtrqekokvd.html

Go:   // 无解构
来源：http://hz.xuanzx.com/gtuyrsvkly.html

Ruby: a, b = pair
来源：http://hz.yongpay.top/gtpbbuzzcq.html

C#:   var (a, b) = pair;
来源：http://hz.zhiwuduotai.top/gtbxqlquqa.html

[C16] 函数 / 方法重载
来源：http://hz.fzhhl.top/gtybehhvhe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtcjidiguf.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtjxgpvjvn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.0kj1m.cn/gtjymvzxja.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gtcuqytpzd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtvwbmccyx.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinyuanbaomall.cn/gtxzopmifc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shzxlz.cn/gthfsoisxs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hysaishi.cn/gtsinvmbbm.html

================================================================================
来源：http://hz.smart0.xyz/gtvnenoxmu.html

D. 数组 / 列表 / 集合
来源：http://hz.sufxvd.cn/gtjkcumomn.html

================================================================================
来源：http://hz.jqgfzy.top/gtncmianux.html

[D01] 创建数组 / 列表
来源：http://hz.fengsongda.top/gtprlyyucd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenzaomai.com/gtzwuszrxk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnqzz.top/gtwwknznuc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxuanxn.top/gtfnveryam.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinghuilouyu.cn/gtlvjfwhzh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.mhx1999.top/gttecynizr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.shangyingyoupin.top/gtgboduhbg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hongshengwenyu.top/gtyzyjuzcg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hongshengwenyu.top/gtdpqyathv.html

[D02] 追加元素到末尾
来源：http://hz.xziqi.cn/gtbydhjvlw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.hongshengwenyu.top/gtmzxbceke.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.pycfn.com/gtutgdmfqw.html

JS:   arr.push(4);
来源：http://hz.316326.xyz/gtrrztcyxt.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtvmmewbhz.html

Java: list.add(4);
来源：http://hz.snrcjt.cn/gtdjrlceww.html

Go:   arr = append(arr, 4)
来源：http://hz.fzhhl.top/gtflhwlaax.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.birdmap.top/gthtgbpbrk.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtpdyhmjqt.html

[D03] 在指定位置插入元素
来源：http://hz.ppjwa.cn/gtgzmjhzrc.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtyfxbhaia.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.nanxinkj.top/gtxrjcjoxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtuzzdkinw.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xuetiantiany.cn/gtvbbhdhxj.html

Java: list.add(0, 0);
来源：http://hz.quarkkingdee.top/gtsghskjwc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.aizwys.cn/gtwnkvlgdv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.kuanghao11.cn/gtttmsuyyx.html

C#:   list.Insert(0, 0);
来源：http://hz.nanxuanxn.top/gtzhedxmov.html

[D04] 删除元素
来源：http://hz.ivvv.top/gtalopyrym.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.sysykeji.top/gtlpeyinqd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.sufxvd.cn/gtmwryzrqq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtelnsgzey.html

TS:   arr.splice(0, 1);
来源：http://hz.xinyue.icu/gtemfyraym.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.cheryme.top/gtdduoxhjf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sxryk.cn/gtvrbikfuv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yj20258888.top/gtaplgypae.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gtotoocyew.html

[D05] 访问与修改元素
来源：http://hz.ivvv.top/gtegiuaiyd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhaomingkeji.xyz/gtpfansfrh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gteetmaikp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.fengsongda.top/gtutobhsxy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zdqjudy.top/gtiqjzagfh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtnidnoile.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtpvsusalx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtzczosoeh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtkbxuynrc.html

[D06] 数组长度
来源：http://hz.cqqwz.cn/gtiilopiqh.html

Py:   len(arr)
来源：http://hz.zhongyouzk.top/gtcfafmmvw.html

PHP:  count($arr);
来源：http://hz.gzhubu.top/gtiapdjerq.html

JS:   arr.length
来源：http://hz.andypj.xyz/gtmthbrngo.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtnkgfrbfk.html

Java: list.size();
来源：http://hz.aibaodan.cn/gtqqjbeuaz.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtkdymqqgt.html

Ruby: arr.length; arr.size
来源：http://hz.hnxiangtu.top/gtkhdauhzm.html

C#:   list.Count;
来源：http://hz.yj202588.top/gtofgnmmqk.html

[D07] 切片 / 取子数组
来源：http://hz.yj202588.top/gtdzrggfob.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.dashuyun.cn/gtxqvpnxen.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shangyingyoupin.top/gtgmhhuokh.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtzainuxnt.html

TS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtjldgwknu.html

Java: list.subList(1, 4);
来源：http://hz.yuanzhike.top/gtwblxfmlw.html

Go:   arr[1:4]
来源：http://hz.wangshuangyany.cn/gttoeiirpk.html

Ruby: arr[1, 3]
来源：http://hz.zhongyouzk.top/gtrexzawxa.html

C#:   list.GetRange(1, 3);
来源：http://hz.pengpengdd.cyou/gthotjalqy.html

[D08] 合并两个数组
来源：http://hz.jqgfzy.top/gtyzerqbfc.html

Py:   a + b;  a.extend(b)
来源：http://hz.hywenlv.cn/gtdrgssugu.html

PHP:  array_merge($a, $b);
来源：http://hz.ywan-chungtsiang.top/gtlaoaofyc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtuqyxbgim.html

TS:   [...a, ...b];
来源：http://hz.yj20258.top/gtzsksveoj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yonumen.top/gttmwlqupm.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gttaoybxnx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtuluqjdhk.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtirsowmyw.html

[D09] 排序（升序）
来源：http://hz.jyoumei.cn/gtgibqmjgs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jyoumei.cn/gtwcneuiev.html

PHP:  sort($arr);
来源：http://hz.pycfn.com/gtpbnosbzr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhongyouzk.top/gtbwbszjix.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuetiantiany.cn/gtcizhshpz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gtkfenczcf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtqqzzadtx.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtqjjrzegx.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtwliuiccp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dianchejie.cn/gtbtwrppcm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.pycfn.com/gtboeeuhcc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jianghu66.top/gtmihvzvqe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtbrdqooou.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gtkbfpqvrw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.vqdsnc.cn/gtppslfoym.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yueranfly.top/gtkaknjitz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.mhx1999.top/gtnimmynyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sxryk.cn/gtqcbzcopa.html

[D11] 反转数组
来源：http://hz.zhiwuduotai.top/gtepzqicso.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.9152youxi.cn/gtamvgtrza.html

PHP:  array_reverse($arr);
来源：http://hz.zhengqikj.top/gtpqviesqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenzaomai.com/gtjtnoevhp.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gtxizpvkvs.html

Java: Collections.reverse(list);
来源：http://hz.pycfn.com/gtmhhdaxtx.html

Go:   slices.Reverse(arr)
来源：http://hz.snrcjt.cn/gtgxvapknv.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtukibrpan.html

C#:   list.Reverse();
来源：http://hz.hnqzz.top/gtmpswrnmt.html

[D12] 查找元素下标
来源：http://hz.c1oappe.top/gtqnyvyyuk.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtarqtlori.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jinghuilouyu.cn/gtdtpifauf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuxming.cn/gtlaoenbtb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtpnrwesyy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuanzhike.top/gtqyhqxokd.html

Go:   slices.Index(arr, x)
来源：http://hz.yj20258.top/gtstbatjxq.html

Ruby: arr.index(x)
来源：http://hz.kuanghao11.cn/gtxztkaenx.html

C#:   list.IndexOf(x);
来源：http://hz.jlsjyb.cn/gtrduuiiuf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jlsjyb.cn/gtqiwowamu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.feifeiyinyue.top/gtlnfagaav.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gotoacloud.top/gtkcwzgcce.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtngsiqjax.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtfrcnyxnc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gaohongyu789.top/gtblnltfud.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yvedp.cn/gtbwgywuoo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gaohongyu789.top/gthkxskemh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenlongwang.top/gtyadlzyxt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtwbcdraue.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxinkj.top/gtclmwbddp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gtjuwgokiq.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gttnhmkjfi.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtydioiznj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yongpay.top/gtnnxvscww.html

Go:   // 手写循环
来源：http://hz.hammf.cn/gtgoqyhklz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gaohongyu789.top/gtyjrtopnd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtjcpzvuzd.html

[D15] 去重
来源：http://hz.yongpay.top/gtxngejfdk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.tianlin.xyz/gtlnolcdkh.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtfjkjndam.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtqevrirfv.html

TS:   [...new Set(arr)]
来源：http://hz.redwolf501.top/gttphkdugy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.haohaochexian.top/gtmgwoczdy.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ivvv.top/gtgomqkpmy.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gtqtnbpnhj.html

C#:   list.Distinct().ToList()
来源：http://hz.hywenlv.cn/gtrrzubsoz.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtzyjpamee.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.tian-w.cn/gtbjjivqal.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hammf.cn/gtnmthidlo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.mhx1999.top/gtgvbbcfbp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tianlin.xyz/gtjbdummxx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgfzy.top/gtzhljnxfn.html

Go:   // 手写循环累加
来源：http://hz.9152youxi.cn/gtuvowyohs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtowdpyjpg.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigfzy.top/gtlozabfwc.html

[D17] 最大值与最小值
来源：http://hz.gotoacloud.top/gteodtbxfe.html

Py:   max(arr);  min(arr)
来源：http://hz.gaohongyu789.top/gtyljgsjqf.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtgqczangx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.havefunace.top/gtaosshhdl.html

TS:   Math.max(...arr);
来源：http://hz.yonumen.top/gtsqkrwmpk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nwbrower.top/gtleaycaas.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhoulong.xyz/gtrdckoadp.html

Ruby: arr.max;  arr.min
来源：http://hz.shanyushiyangkeji.top/gtliilfavd.html

C#:   list.Max();  list.Min()
来源：http://hz.hfpthk.cn/gtxqjqrgpd.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gtexnycwwb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhongyouzk.top/gtkqldcjcv.html

PHP:  array_merge(...$nested);
来源：http://hz.meibo888.top/gtfwhpfwha.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtehqpabno.html

TS:   nested.flat();
来源：http://hz.shanyushiyangtech.top/gtcwoeroto.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtfhamjfel.html

Go:   // 手写双层循环
来源：http://hz.kuanghao11.cn/gtixaxygta.html

Ruby: nested.flatten
来源：http://hz.52xcode.cn/gtvbndigfd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtllpzeczc.html

[D19] 按字段分组
来源：http://hz.jiagoushi.top/gtimnvgqtb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.haohaochexian.top/gtngztpfaw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.vqdsnc.cn/gtitrniglk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sysykeji.top/gtwpfyzzfb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yueranfly.top/gtlzwgcuob.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gttlodsrxc.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtfqbqosuq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shzxlz.cn/gtlzfbirfg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtrqgwlncu.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtpgdyfymw.html

Py:   Counter(arr)
来源：http://hz.cqqwz.cn/gtdhsvrgvd.html

PHP:  array_count_values($arr);
来源：http://hz.zhijiandao.cn/gtdfuguply.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.kuanghao11.cn/gtnknkcfui.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtjosobiwj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtnsqfcoqk.html

Go:   // 手写 map[T]int
来源：http://hz.yvedp.cn/gtmrrxsapo.html

Ruby: arr.tally
来源：http://hz.ppjwa.cn/gtwqxcsazp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinghuilouyu.cn/gtcdoywmpf.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gtfzsuoqmu.html

Py:   x in arr
来源：http://hz.jinghuilouyu.cn/gtxqqvbsuv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hfpthk.cn/gtlmlynbto.html

JS:   arr.includes(x)
来源：http://hz.wangdashe.top/gteknlsugz.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtmalqeafx.html

Java: list.contains(x)
来源：http://hz.yanxiufei.cn/gtncbjrjmm.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtuksjpjdz.html

Ruby: arr.include?(x)
来源：http://hz.gzhubu.top/gtzgrpvecz.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtoxjaoztn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtttfwcjgp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj202588.top/gtfounfyhd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gtcrmiivfw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.tianlin.xyz/gtezkhhttu.html

TS:   [...arr];
来源：http://hz.haohaochexian.top/gtmgbuwxgm.html

Java: new ArrayList<>(list);
来源：http://hz.sxryk.cn/gtkgtvuwoa.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtleyjzcvn.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ppjwa.cn/gtqzexrnjo.html

C#:   new List<int>(list);
来源：http://hz.zdqjudy.top/gtijrbyvba.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gthuygxnzd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.316326.xyz/gtiwzntpha.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.vqdsnc.cn/gtfxzseuju.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.svipenyu.cn/gtgoohpycm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yvedp.cn/gtnvufqmlm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhijiandao.cn/gtvkzcqzca.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtnmfrcpiz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.andypj.xyz/gtdqwosebq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yongpay.top/gtjgdtgckt.html

[D24] 字典 / Map 基本操作
来源：http://hz.redwolf501.top/gtgqjjbaxf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtxvwamfcr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinghuilouyu.cn/gtmlxpnqnk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.cqqwz.cn/gtxbfzwqeq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.andypj.xyz/gtezyioheu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.sweek.top/gtjmigpxte.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.mhx1999.top/gttjvsuwhk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gzhubu.top/gtwseypaut.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ehwqpu.com/gtzzndtnnd.html

[D25] Set 集合去重与交并差
来源：http://hz.kuanghao11.cn/gtxjmzlmpq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yuanzhike.top/gtlubwwvuo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtiqeusrcc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hywenlv.cn/gtsfoqlzyy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtobsdyexl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guowangkeji.top/gttmgvdkco.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.havefunace.top/gtdmhykeza.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nwbrower.top/gtjrvuuycg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gzhubu.top/gtgqrgkeiw.html

[D26] 数组转字符串
来源：http://hz.cqqwz.cn/gtpqiqltxn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ppjwa.cn/gtndbptyas.html

PHP:  implode(", ", $arr);
来源：http://hz.sufxvd.cn/gtvepplfwg.html

JS:   arr.join(", ")
来源：http://hz.chenlongwang.top/gtusumbqwc.html

TS:   arr.join(", ")
来源：http://hz.shuidangran.top/gtzkezlsoh.html

Java: String.join(", ", list)
来源：http://hz.dashuyun.cn/gtultslpsj.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zycfv.cn/gtjdywyaip.html

Ruby: arr.join(", ")
来源：http://hz.shzxlz.cn/gtdpxpgdqc.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtdifpyipi.html

================================================================================
来源：http://hz.fengsongda.top/gtmyzdtlrj.html

E. 字符串处理
来源：http://hz.hnqzz.top/gtyakuljuu.html

================================================================================
来源：http://hz.jiagoushi.top/gtziibbxeb.html

[E01] 拼接字符串
来源：http://hz.shangyingyoupin.top/gtvbwytwie.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhixingplan.top/gtlfhpwnoq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.ybcxt.top/gtqpcumfvi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shanyushiyangtech.top/gtuxmfurpp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sxryk.cn/gtazryysgi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydzc1.top/gtukptzige.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.0kj1m.cn/gtwhcihicl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.mhx1999.top/gtntzysdpn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yuxming.cn/gtzilzztsq.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtngivowxx.html

Py:   "ab" * 3
来源：http://hz.shangyingyoupin.top/gttftgxpey.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhongyouzk.top/gtcsgtsrco.html

JS:   "ab".repeat(3)
来源：http://hz.jinqigfzy.top/gtiugbbiea.html

TS:   "ab".repeat(3)
来源：http://hz.xinyue.icu/gtxicquhme.html

Java: "ab".repeat(3)
来源：http://hz.chenzaomai.com/gtcugsepgt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtcwuynyab.html

Ruby: "ab" * 3
来源：http://hz.meibo888.top/gtuqeuwcin.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gaohongyu789.top/gtxazwtzxl.html

[E03] 截取子串
来源：http://hz.zhiwuduotai.top/gtjfssuhqg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtlczsxhfe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhijiandao.cn/gtbugfpxag.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtwkkmeppq.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtqvdlfevm.html

Java: s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtujsfqnex.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hammf.cn/gtconxzqjd.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.iojbl.cn/gtcenfxujc.html

C#:   s.Substring(1, 3)
来源：http://hz.hnxiangtu.top/gtpdsdhplm.html

[E04] 查找子串位置
来源：http://hz.shuidangran.top/gtckjbkfpw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hongshengwenyu.top/gtzjmoypue.html

PHP:  strpos($s, "x");
来源：http://hz.jiagoushi.top/gtfdrfhqcv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yongpay.top/gtfoouvlks.html

TS:   s.indexOf("x")
来源：http://hz.sxryk.cn/gtuagxgkzb.html

Java: s.indexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtotfcqmkl.html

Go:   strings.Index(s, "x")
来源：http://hz.shanyushiyangkeji.top/gtinfxdlht.html

Ruby: s.index("x")
来源：http://hz.shzxlz.cn/gtixsegpcn.html

C#:   s.IndexOf("x")
来源：http://hz.wangdashe.top/gtoivucphz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.vqdsnc.cn/gtsjvhtfdp.html


<!-- 参考信息 -->