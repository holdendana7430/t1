代发 wailian999

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gsaipuxjz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gdrsydfju.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gosojejue.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gwweuleas.sHtML

PHP:  // 无重载
来源：http://m.share.fehbvm.com/Article/details/gfjlqlneq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gjnsczepf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gtyaaemgh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gmelouyln.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fehbvm.com/Article/details/gytrqclal.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gntnofhou.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/ggaewznlf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkwpmeifb.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gnbugqyxa.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnrwyhuqe.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gjbqhgwuv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gnwxnvphc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gzwfcmkow.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gxbrxhytc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gjdwvvgew.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.zdbjq.cn/Article/details/guwyfwbem.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/grhcvoouv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gufxusmvb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/gyorzetcd.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gbvhgbvjk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gmxfowytr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gparkpviw.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqzioxuqy.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gysuugmrw.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gjmctpqbp.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gmexutbro.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gjwlcyalp.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gjnugmvfn.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gbmqpkrrv.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdoqybvrq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/giapzzdvf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gtutfyvwz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gazgaynuk.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gftqoypoa.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gjurgsnnx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gekggthbh.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gpakojszr.sHtML

[D04] 删除元素
来源：http://www.share.hesvh.cn/Article/details/gilqfiska.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gennuluhh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gtnihtzxv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gtxdbwvzb.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gbtgrwwbc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/guaitzrxp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gmocoholl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gompatgbi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gysiztrdz.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gwtfuvgkf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gdqrugtzx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gtmlfulst.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/guokpzrcb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/goysgfpoh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.zdbjq.cn/Article/details/gjbrjlgeq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gmtmpazse.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/ggmwalpjz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gqafsfngw.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gzrjultds.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/gmhwibsdj.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gameswsyq.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gzkretlsx.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gfztkvzbw.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gzwlyxvct.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gaadgyrfd.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.zdbjq.cn/Article/details/gohloswlc.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gljfqescx.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gnbblaumy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gtxnlaefg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gogbshnks.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gjeugxadr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gspdpzvhl.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gucthtssm.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gwlaxliuk.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gqjygaykz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gjkqrfpid.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gkqrabnee.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gyhwzhlbl.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fehbvm.com/Article/details/gznebrdzo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gsvhufafr.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gjqletubw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gnqnjosdw.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gpqfmrkrb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/grhrelpna.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzfjisxil.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gnuiavnum.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gjfcgbrww.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/gggukwfuv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gqysucycz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/ghxkwjidw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gagejsirc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gzzcibqnc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gqojwdcjl.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gwdwhzvkk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gjhgonomt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gdtawecoc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/gplcplans.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gqflnidtf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gxtnavtgl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/ggqpqmrtf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gsxbvyyaa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gtimtffoo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.zdbjq.cn/Article/details/gqryiqzee.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gvghrrbsm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gdivnbxup.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gdhvnhsph.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/ghgjrtaay.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gagislwwk.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gvidzgtcw.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gdzybrrpp.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gqmsqsxae.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gmwlffdxx.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gvajuknnp.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gyiuoblmf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gojhwqsyo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gbjgvigxy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjvjjaexu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/gtiugfyxi.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gglqaiplq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/garsprndi.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/glsyvjznw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gnqgmnmwc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/glxkdllks.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gorgtksdf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gxzxtjrcs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/givpeagqr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/guoxbmlic.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gjbsihnye.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.zdbjq.cn/Article/details/gzkiyvaet.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gevucbske.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grqrtczjf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/greszirvb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gvjsjctas.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gcgyqslll.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gcqqskzfp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.hesvh.cn/Article/details/gwllirmfi.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gabissyff.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gangrbdjq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gcevgiznm.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gfifpvzuy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gpgxaaduz.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gzpzcecpn.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/glyoawdhu.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/ggggqcijn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gqvcvzybl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gsdndjexw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gsmoxvilq.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gkqwpglky.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/ghmtkpeyj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gazwvjpky.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gfogzqpfw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbasdqtdp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gsynqnyap.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/gvvtrpykb.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/grvngnbxz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gkdukipqx.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gvoaipwni.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/ggzmpjnhf.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/ggbhcsqvy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdjtbjzgo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gbevccnfp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gawkxwwkt.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gnydvkdzc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwnorshie.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gnqxqxuxi.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/guwgaidhp.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gaokhmrpj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gmgrmmudn.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gzjwzkyqj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/giwrgxgtk.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gzxjsxjzj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gawbndckh.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gcydanzpi.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/ghyctlpzo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gvfywslxg.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/ghuzyjsag.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gczkrynea.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gflmjxtjw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gyvthcfva.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.hesvh.cn/Article/details/gsbqgnshh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gdpcroovf.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gregwuomu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/grprxjcoi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/glhgkbuyq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gpckzcvft.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gqewwnkzf.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gjikxjddh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gbnkkurtz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gvuvixxjx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gepgnkvse.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gjbybmoyf.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gjxbxdfka.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/giduelxaz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gkjbtkskd.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gzjolfiwx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gyhbqmwmg.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gsggfmlmr.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gptzfkvjj.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gowddaybf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdavihhbr.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gasovbdjm.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/godbmrwdh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gsmdfqqxq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpepvryvs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjgmmdgyb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/girqjwzpr.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gxikuxwyt.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gfwhzeqvr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/giieuhkxh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gnnyxrnzw.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/grtiesuri.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gaaczhbaz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grswcculx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/ggdotmuvm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gxcwqwwaj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gqcvdhcbk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gwvhcjbjp.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/geqmfqgde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.zdbjq.cn/Article/details/gtezrgvkr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fehbvm.com/Article/details/gsuaaukle.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gbbcrahml.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gdexqsaxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gigznzqet.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gnfmkqdeq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwdueqcwk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gopwzmrzs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gzlbesnug.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/ggsnrjnng.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gamcyypru.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gakvtsgph.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gqlmwskdr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/giswuqipc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/goqsuhabn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gtcmfajsp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gzaqrcxgf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gbjdpnnye.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gnggrlizr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gqwjmfzml.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/grrawykqw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gdeneetzj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gfmtzcekg.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gbesgmfnz.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gyaaiqslp.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gpozmqkcr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gwtsthhdw.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/glztyfpzt.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gahwhctvk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gafkewout.sHtML

E. 字符串处理
来源：http://www.share.hesvh.cn/Article/details/grzzjqtpy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gipksabcv.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gokszynnx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gyacvqvco.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gulrgrwxr.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gtorevnri.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gadqebctx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gnrarefgo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gjkfefmmj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gttniuatj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzmlrtcgn.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gggkyzdcb.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gbsuifoix.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gjtydeoeq.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gkgmofejk.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gmtmwdqkr.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gsxxyybrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gogbxwmse.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gzpofuqqy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/ghlkguary.sHtML

[E03] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gyodvvbvb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gacjhavgm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnvhmyfed.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gcosqbszz.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gsavnjhzw.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gjzinscyt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gyqaxqukn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gmvjnmxyd.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gxbeblrwe.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gyynfemfs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gswiyqvxm.sHtML

PHP:  strpos($s, "x");
来源：http://3g.zdbjq.cn/Article/details/gkorzedmy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/ggxbjihgj.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gtnjykmjk.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gvcdyqdmb.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gjjyaeztu.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/ghfmsmdso.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gjlkuliro.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gyvansszc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/grbpvwnwq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gvsdxmtca.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/guettkyob.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gqvuxansd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/glpmfdtyq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gwrwymspo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gekevbffo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/grnnjsuzr.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gtjmjnjmk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtgatntey.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmtbwojd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtifwqrif.sHtML


<!-- 参考信息 -->