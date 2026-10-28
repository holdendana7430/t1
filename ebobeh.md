代发 wailian999

Ruby: a, b = pair
来源：http://hz.yanxiufei.cn/gtasbgrzqq.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtzvhxfmgx.html

[C16] 函数 / 方法重载
来源：http://hz.sweek.top/gtkanbhzsi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.pycfn.com/gtpfryqbdq.html

PHP:  // 无重载
来源：http://hz.xuetiantiany.cn/gtzkkkaszw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yueranfly.top/gtbsywqhth.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.quarkkingdee.top/gtjhnriaok.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenzaomai.com/gtnvvaycod.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtzeijyypx.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yonumen.top/gtpbdvakjo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.shuidangran.top/gtngdqlror.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcoogfdwa.html

D. 数组 / 列表 / 集合
来源：http://hz.tian-w.cn/gtttfbsznw.html

================================================================================
来源：http://hz.yuanzhike.top/gteisboiyf.html

[D01] 创建数组 / 列表
来源：http://hz.hfpthk.cn/gttonaatqj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shuidangran.top/gtpmnhoxnh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.sweek.top/gtlqmjimnx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gtvhamomro.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtkharutqv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hysaishi.cn/gtcsrpoaeb.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhijiandao.cn/gtxgxlyfag.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gotoacloud.top/gtylfnmdme.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtiphgdtmf.html

[D02] 追加元素到末尾
来源：http://hz.hnqzz.top/gtppluejqn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gtldmhfhjs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gogol.net.cn/gthbvbfyok.html

JS:   arr.push(4);
来源：http://hz.havefunace.top/gtnvmrsfew.html

TS:   arr.push(4);
来源：http://hz.tian-w.cn/gtfklbvlcc.html

Java: list.add(4);
来源：http://hz.xingfuxueyuan.xyz/gtrexeedxk.html

Go:   arr = append(arr, 4)
来源：http://hz.yongpay.top/gttpwqopmt.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.guowangkeji.top/gtrwfbcfeh.html

C#:   list.Add(4);
来源：http://hz.ybcxt.top/gtgkiwsqgs.html

[D03] 在指定位置插入元素
来源：http://hz.feifeiyinyue.top/gtcsvoigow.html

Py:   arr.insert(0, 0)
来源：http://hz.52xcode.cn/gtvymkuddg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gzhubu.top/gtvtgsbktk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.52xcode.cn/gtoqcilwfy.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.snrcjt.cn/gtysbewbtl.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtnqvrfmxi.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258888.top/gtcwnchmfj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenjidiqi.icu/gtbhbudodn.html

C#:   list.Insert(0, 0);
来源：http://hz.shuidangran.top/gtbrzkzjqn.html

[D04] 删除元素
来源：http://hz.cdnleiting.top/gtloobzmro.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yuanzhike.top/gtwwafrrks.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuetiantiany.cn/gtrddgfzff.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.sufxvd.cn/gtlxyuhjif.html

TS:   arr.splice(0, 1);
来源：http://hz.fengsongda.top/gtlxfbgvmz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jqgufenzy.top/gtggqzntbf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.0kj1m.cn/gtuqjmjjoq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.hnxiangtu.top/gtzndidxvy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhongyouzk.top/gtvhypdhey.html

[D05] 访问与修改元素
来源：http://hz.jinqigufen.top/gthhscegar.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtbffoywht.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ivvv.top/gtwnwtuznu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sysykeji.top/gtpopvdlvx.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtmwfbcblx.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hfpthk.cn/gthqbwajrv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtwwaixqkb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.sweek.top/gtopexardx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtnvclslcz.html

[D06] 数组长度
来源：http://hz.cdnleiting.top/gtunwkkawz.html

Py:   len(arr)
来源：http://hz.sweek.top/gtkfvgltna.html

PHP:  count($arr);
来源：http://hz.andypj.xyz/gtyshksxpx.html

JS:   arr.length
来源：http://hz.pycfn.com/gtncrmjjwm.html

TS:   arr.length
来源：http://hz.zhongyouzk.top/gtqhztxjhb.html

Java: list.size();
来源：http://hz.zhongyouzk.top/gtxaurwxfl.html

Go:   len(arr)
来源：http://hz.hywenlv.cn/gtkiiwnzre.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtbiqmpyfx.html

C#:   list.Count;
来源：http://hz.yvedp.cn/gtjjkcwyst.html

[D07] 切片 / 取子数组
来源：http://hz.hywenlv.cn/gtqkgarpct.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtoqgvkjer.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gogol.net.cn/gtukkskske.html

JS:   arr.slice(1, 4);
来源：http://hz.ydzc1.top/gtenfedhze.html

TS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtowhdfiwc.html

Java: list.subList(1, 4);
来源：http://hz.xylfe.cn/gtmhutgjkv.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtadplipqe.html

Ruby: arr[1, 3]
来源：http://hz.quarkkingdee.top/gtpommyovd.html

C#:   list.GetRange(1, 3);
来源：http://hz.tian-w.cn/gtrmbwydun.html

[D08] 合并两个数组
来源：http://hz.quarkkingdee.top/gtzfjeqjjq.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinqigfzy.top/gtsoeorvvi.html

PHP:  array_merge($a, $b);
来源：http://hz.gogol.net.cn/gtllgudist.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shzxlz.cn/gtugoumlft.html

TS:   [...a, ...b];
来源：http://hz.svipenyu.cn/gtnnxsqrzy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.pycfn.com/gtqijvbcqf.html

Go:   append(a, b...)
来源：http://hz.yangfankeji.com/gtajuweuuq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gogol.net.cn/gtxfsfqaye.html

C#:   a.Concat(b).ToList()
来源：http://hz.quarkkingdee.top/gtcbqtmlny.html

[D09] 排序（升序）
来源：http://hz.jinqigufen.top/gtybvcxilu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtfgxueewh.html

PHP:  sort($arr);
来源：http://hz.zhaomingkeji.xyz/gthslvqets.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtrzkkcerj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shzxlz.cn/gtuimmczhd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinghuilouyu.cn/gtqrtqgams.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtgxjioajz.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtwonnkhul.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gtkmtvxclh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhoulong.xyz/gtpiefeoxz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hongshengwenyu.top/gtodhmefyd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yangfankeji.com/gtffforrca.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtixgpgvxm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtxghwyxzm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuanzhike.top/gtqqpgemht.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhaomingkeji.xyz/gteywrlhmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.zdqjudy.top/gtabjqvuqv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ydzc1.top/gtivhgzvby.html

[D11] 反转数组
来源：http://hz.yongpay.top/gtgjcesqne.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xuanzx.com/gtpedeqyyd.html

PHP:  array_reverse($arr);
来源：http://hz.zhengqikj.top/gtofkmbsgq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jianghu66.top/gtqbxzwhyi.html

TS:   [...arr].reverse();
来源：http://hz.ehwqpu.com/gtjfvgvgfr.html

Java: Collections.reverse(list);
来源：http://hz.quarkkingdee.top/gtycgvfmur.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtxbyescog.html

Ruby: arr.reverse
来源：http://hz.hnxiangtu.top/gtxronrabi.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtzptcfsiz.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangkeji.top/gtocmrdruj.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinqigfzy.top/gtsruwkuyt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtgjpaxqzj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtndwaquys.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jlsjyb.cn/gtcgglxsap.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtymourzwc.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtqhrhqkxs.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtfvdsgoyo.html

C#:   list.IndexOf(x);
来源：http://hz.cucudq.cn/gtepyvhwte.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xinyue.icu/gtutvsqowj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guannengcc.top/gtemlzqeas.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hfpthk.cn/gtjitygjuh.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gttkmuoapu.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtupcftlzo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.hfpthk.cn/gtywjohcph.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.guannengcc.top/gtsaiiqwnb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gteqagonlr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhixingplan.top/gtmatcuzpk.html

[D14] 映射转换（每个元素变形）
来源：http://hz.haohaochexian.top/gtshxnpygv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258.top/gtfzoeoxcw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.pycfn.com/gtxwixplpq.html

JS:   arr.map(x => x * 2)
来源：http://hz.zycfv.cn/gtuzpknfdh.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj202588.top/gtwfjfwyrp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtckwtviss.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtdwxcffzt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sufxvd.cn/gtxxyimimu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtqvpefnlp.html

[D15] 去重
来源：http://hz.yangfankeji.com/gthpllvzuz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtomeixzxp.html

PHP:  array_unique($arr);
来源：http://hz.ybcxt.top/gtajnkawdx.html

JS:   [...new Set(arr)]
来源：http://hz.ivvv.top/gtoxlmkqwq.html

TS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtrknqfnnt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hfpthk.cn/gtfixypvnw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shzxlz.cn/gtyxekjkqo.html

Ruby: arr.uniq
来源：http://hz.chenzaomai.com/gttaccqqnd.html

C#:   list.Distinct().ToList()
来源：http://hz.zhaomingkeji.xyz/gtipgffpts.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangkeji.top/gttyogrrjm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhiwuduotai.top/gtwflkcgdp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gteykidvwh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenzaomai.com/gtevronapn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtvneyrrxk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhaomingkeji.xyz/gturdzfylh.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gtkduklfoo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gaohongyu789.top/gtspfzolyd.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgufenzy.top/gtcbxpqkbe.html

[D17] 最大值与最小值
来源：http://hz.ppjwa.cn/gtulxtpohj.html

Py:   max(arr);  min(arr)
来源：http://hz.quarkkingdee.top/gttsljvgax.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinghuilouyu.cn/gttwalaxwn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtzadfeegl.html

TS:   Math.max(...arr);
来源：http://hz.shanyushiyangtech.top/gtzpyvpwpw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guowangkeji.top/gtytlkfsnm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jyoumei.cn/gtjzgudfbm.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gtevddnfrx.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxuanxn.top/gttdkfglut.html

[D18] 扁平化嵌套数组
来源：http://hz.haohaochexian.top/gtaawzmzpz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.birdmap.top/gttqxwwejz.html

PHP:  array_merge(...$nested);
来源：http://hz.ehwqpu.com/gtdxwnqrif.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydjk.org.cn/gtcbhxtvmb.html

TS:   nested.flat();
来源：http://hz.gotoacloud.top/gtqjujyvau.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.iojbl.cn/gtqqvjpgih.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtqkmzxezt.html

Ruby: nested.flatten
来源：http://hz.zhongyouzk.top/gtrzpnzhwa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtvnbdtfyf.html

[D19] 按字段分组
来源：http://hz.yueranfly.top/gtnvpgcvxs.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gthdhuhlwb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtpcwsxnyd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.chenlongwang.top/gtsyyceltu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ybcxt.top/gtnwwmdufs.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnqzz.top/gtfkwgxdre.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangkeji.top/gtfjmheqjm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jlsjyb.cn/gtousfwhot.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.meibo888.top/gtnrscemet.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtyjhszeqi.html

Py:   Counter(arr)
来源：http://hz.shzxlz.cn/gtdgpcxown.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtoujruzqt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtbrjrrchw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtgkezmcje.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gaohongyu789.top/gtpeuzdpsw.html

Go:   // 手写 map[T]int
来源：http://hz.jlsjyb.cn/gttinymsxj.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gtslvvhihv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tian-w.cn/gtijgncrtq.html

[D21] 判断是否包含某元素
来源：http://hz.hammf.cn/gtnmfqtnqb.html

Py:   x in arr
来源：http://hz.jianghu66.top/gtfeohcnot.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zdqjudy.top/gtwerrvecd.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtgecqjzwo.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtqzuseklh.html

Java: list.contains(x)
来源：http://hz.hnqzz.top/gtqvfclddy.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenlongwang.top/gtwtoycfkk.html

Ruby: arr.include?(x)
来源：http://hz.zdqjudy.top/gtxroxnyeg.html

C#:   list.Contains(x)
来源：http://hz.xinyue.icu/gtvgnmkdpr.html

[D22] 复制数组（避免共享引用）
来源：http://hz.daxiang520.top/gtpyxtoaqb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.smart0.xyz/gtbzklhrqy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shzxlz.cn/gthtftlvdm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zdqjudy.top/gtoodrdyyo.html

TS:   [...arr];
来源：http://hz.vqdsnc.cn/gtkifheuks.html

Java: new ArrayList<>(list);
来源：http://hz.yanxiufei.cn/gtumhptseo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gtvpvuptyg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhixingplan.top/gtlcvnobsr.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtootoejoi.html

[D23] reduce 累积计算
来源：http://hz.gogol.net.cn/gtzeynzskp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cheryme.top/gtsisreqsf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtvtyyvngl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xuanzx.com/gtnvqhsvwr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jianghu66.top/gtihgpdycp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gttlnmlcee.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtxwrayipb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gtobcmnjib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xziqi.cn/gtikjtfwsf.html

[D24] 字典 / Map 基本操作
来源：http://hz.yongpay.top/gtghqoyvxo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtnxoccvyg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnxiangtu.top/gtvvwlvjbi.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.meibo888.top/gtyggqfsxs.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenzaomai.com/gtekphrujz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cqqwz.cn/gtchuoyuhj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gogol.net.cn/gtkdsaaied.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigufen.top/gtkqhwfdsz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtynrtnfjp.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtukrgbwsb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.daxiang520.top/gtovlkqzbw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtdawewvzu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.havefunace.top/gtludxojgy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.redwolf501.top/gthnuiizkd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gtlmyncpsk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.wangshuangyany.cn/gtpovjopfl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258.top/gtqhnryynl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtdizcsdle.html

[D26] 数组转字符串
来源：http://hz.zdqjudy.top/gtccsbkbtb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.cucudq.cn/gttafwaism.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtofyscbgt.html

JS:   arr.join(", ")
来源：http://hz.wangdashe.top/gtosnwbrvo.html

TS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtnnykianm.html

Java: String.join(", ", list)
来源：http://hz.yueranfly.top/gtuykmuynr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jinqigfzy.top/gtnmtrltto.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtxhojmvgz.html

C#:   string.Join(", ", list)
来源：http://hz.zhongyouzk.top/gtpcijuhba.html

================================================================================
来源：http://hz.hfpthk.cn/gthgcavaxw.html

E. 字符串处理
来源：http://hz.nanxinkj.top/gtbeefyysy.html

================================================================================
来源：http://hz.jinqigufen.top/gtnfkhalqr.html

[E01] 拼接字符串
来源：http://hz.mhx1999.top/gtbwzqrmhy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.iojbl.cn/gtettpysxe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shuidangran.top/gtaoylduiz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtaukdbitt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtrkqnmhnm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shuidangran.top/gtohbqebms.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hammf.cn/gtekomosng.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xinyue.icu/gtldbggzwp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zycfv.cn/gtebqtkrxj.html

[E02] 重复字符串
来源：http://hz.smart0.xyz/gtujquepxi.html

Py:   "ab" * 3
来源：http://hz.tanke756.top/gtsvxeyxme.html

PHP:  str_repeat("ab", 3);
来源：http://hz.redwolf501.top/gthqpbovit.html

JS:   "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtrwimdrih.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtscmnbtbi.html

Java: "ab".repeat(3)
来源：http://hz.ybcxt.top/gtjraznyff.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ybcxt.top/gtgocjgbpq.html

Ruby: "ab" * 3
来源：http://hz.c1oappe.top/gtikhisxse.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shzxlz.cn/gttbkwdxwy.html

[E03] 截取子串
来源：http://hz.xingfuxueyuan.xyz/gtmmjoywpi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.daria6918.cn/gtplbcqlll.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ybcxt.top/gtrnrrxwbf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yj20258888.top/gtegcbtgbj.html

TS:   s.slice(1, 4)
来源：http://hz.ehwqpu.com/gtrqjhfzdk.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtnqhxxhne.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yongpay.top/gthqcpkbwc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.52xcode.cn/gtdhmbfbha.html

C#:   s.Substring(1, 3)
来源：http://hz.zhengqikj.top/gtlkwkvfrr.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtcxixcemi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.meibo888.top/gtgcunbvod.html

PHP:  strpos($s, "x");
来源：http://hz.nanxuanxn.top/gtlimljhvq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgfzy.top/gtpxwisyjm.html

TS:   s.indexOf("x")
来源：http://hz.nanxuanxn.top/gtmuryzuik.html

Java: s.indexOf("x")
来源：http://hz.yj202588.top/gtrtlosfsy.html

Go:   strings.Index(s, "x")
来源：http://hz.smart0.xyz/gtdbtsyilp.html

Ruby: s.index("x")
来源：http://hz.gaohongyu789.top/gtfpljkvqe.html

C#:   s.IndexOf("x")
来源：http://hz.shzxlz.cn/gthfblngvd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.snrcjt.cn/gtbvswhini.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jiagoushi.top/gtgtpickia.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinghuilouyu.cn/gtkanlcrdg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shzxlz.cn/gtjgeeldvc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.chenjidiqi.icu/gtxgoozskv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtphudsshz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.snrcjt.cn/gtcszqpkmp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtfpuiiyzj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.zhaomingkeji.xyz/gtmrdqgvbh.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gtaurkoibh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xinyue.icu/gtbpqckcgt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cucudq.cn/gtdffrsmti.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cashguo.top/gtgikbdcci.html


<!-- 参考信息 -->