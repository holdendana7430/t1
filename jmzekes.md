代发 wailian999

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapylcjec.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gofnrkeqt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvfenknt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gragnnboz.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfhmchav.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxwcjbrj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gevnfotaa.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkakoftmt.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gjjepjyfz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbjjmaluk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fanxiaobao.xyz/Article/details/glygiesyz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqznrrmq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/glhdzpsfh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpnawlhi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxmenqkr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjhwyirj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gbtxorhgy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkujqwfm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fanxiaobao.xyz/Article/details/gbfkljdid.sHtML

[D02] 追加元素到末尾
来源：http://baike.fanxiaobao.xyz/Article/details/grtfcvfza.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/gvfloqenr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbprowsej.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/ggmlmubgc.sHtML

TS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcfxqggu.sHtML

Java: list.add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gitytubeg.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfqqzftz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fanxiaobao.xyz/Article/details/gzncvongv.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gffafvddg.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsdobxqs.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/guxluefup.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpfhfwfh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnrztojp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gevuachpk.sHtML

Java: list.add(0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gmwkrdaqc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmxbhos.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqydjjdq.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtmcadsc.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/grzrgxfbz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gytvvfazm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/giwnegzur.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gmxizucjk.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gzygwfgjc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjwaprbn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fanxiaobao.xyz/Article/details/gkycaicrj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfubtreg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.fanxiaobao.xyz/Article/details/giexrrsys.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawoxuey.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhkohthr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gmrbayhgz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjwbbtvg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fanxiaobao.xyz/Article/details/gnmamftmv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gleiswtse.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdfiopin.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gzkobxizl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/glngfqtfx.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyjwebud.sHtML

Py:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gahepjqlw.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gzktdvdqg.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqqrthrc.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojpgbloy.sHtML

Java: list.size();
来源：http://blog.fanxiaobao.xyz/Article/details/gkfefzjvp.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gnceyoymf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gsatsonzm.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/ggmrhrtar.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gazgyteuk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fanxiaobao.xyz/Article/details/gdvrdxhop.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsrctucim.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprwsmckj.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhmurqeh.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatbvgftx.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gavfuxrxp.sHtML

Ruby: arr[1, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gnamwzxoz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcabuppu.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gymeknngk.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fanxiaobao.xyz/Article/details/ggzqwbbxo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnxrggyf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbmpoein.sHtML

TS:   [...a, ...b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gudxyaolz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxkzznob.sHtML

Go:   append(a, b...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxvizsqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgaaezoh.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfqllmtc.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gkjwrvkdn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fanxiaobao.xyz/Article/details/gamamcovv.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkvvwqdf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/guubxolcd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gxevdgypg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnnxmrwn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxtjcvce.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaydujmy.sHtML

C#:   list.Sort();
来源：http://blog.fanxiaobao.xyz/Article/details/gbqtuvlva.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsoukpurm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvzblmfl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gaglgivmh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gsvkkthfo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/ggfhscbbr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gnmkhdjek.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fanxiaobao.xyz/Article/details/gtkggnlih.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkypbljsc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/gaxcmgvcx.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gqawsrqjc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fanxiaobao.xyz/Article/details/gczdcraoa.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/giijzgusw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/ghugtqaqx.sHtML

TS:   [...arr].reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gyaspcoey.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvhudtvy.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gopaxyldc.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gevdpmvxt.sHtML

C#:   list.Reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gggbihain.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqoobwv.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gzafwqknp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gszkrkvml.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxynlavb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjchbytsw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysaexqvr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcqhadrh.sHtML

Ruby: arr.index(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcncwpgd.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjoqasvs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/gruflpawz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gumsrhkqh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfrtwiya.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggflhhktr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyzglzsy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxrjzczi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fanxiaobao.xyz/Article/details/gereqfepk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklstjapt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guusugael.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fanxiaobao.xyz/Article/details/gkxeemoew.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxvrirfu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdjwfikg.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggkbjjeuz.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbyxieo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtvbpjasa.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghexjvujg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/ganxiqygd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhhwtjxv.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gsesqigqo.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gijefofqd.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxexowocg.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gykstaylr.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gzfnmvrul.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzglagfk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxiiiblj.sHtML

Ruby: arr.uniq
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrylhken.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/glhtrckph.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gshcwpwex.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gpfspyixo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gnhfbiecg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrwdpxmm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjoviqtpu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzfinsc.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/ggiwnnacd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gntybawob.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godmwqddz.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/goupgdcfe.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxkterig.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmwkfncz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbzvsfef.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwagutal.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gvxojwsam.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gomatloxj.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/glnwlkrou.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmruwsav.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiyycudk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fanxiaobao.xyz/Article/details/grjmspzgj.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fanxiaobao.xyz/Article/details/gqqicxogs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fanxiaobao.xyz/Article/details/glhoceqoq.sHtML

TS:   nested.flat();
来源：http://m.share.fanxiaobao.xyz/Article/details/glcssxuaf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gogvgxpcf.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaumquvc.sHtML

Ruby: nested.flatten
来源：http://3g.fanxiaobao.xyz/Article/details/gzfamcgkl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwqffpse.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkhvvvwe.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/ganlxjfdj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjxbcezf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fanxiaobao.xyz/Article/details/gmlddfcpp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gkfjudriq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.fanxiaobao.xyz/Article/details/gpyvwloch.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvrxbfpg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrwkbfvx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fanxiaobao.xyz/Article/details/gfuyzrmuw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gukptmoxa.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grryfebbb.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gophhtpoh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gityjhptb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/gjtsksswf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fanxiaobao.xyz/Article/details/gojanodlx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gebdfysqh.sHtML

Ruby: arr.tally
来源：http://m.share.fanxiaobao.xyz/Article/details/ggieqakjo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhaucfi.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjewtarog.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gnbmafvzb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/gfgfsejez.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcowsxxq.sHtML

TS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gxebuedxs.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/grnrxqlpl.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrozrqqb.sHtML

Ruby: arr.include?(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gyosyyvbn.sHtML

C#:   list.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gijnwzmiy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girevmndq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gljgrmwpe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyrebwfg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gjwcucyzl.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfpzkcqm.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gnqlqsabw.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfdgcplm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fanxiaobao.xyz/Article/details/gxpoymsne.sHtML

C#:   new List<int>(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggppyiebu.sHtML

[D23] reduce 累积计算
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrjbmnq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/guffltpxr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuteblln.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gwelbwdfd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnsjheqp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnnfhszc.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwcyhhsd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fanxiaobao.xyz/Article/details/grgxoedez.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcykshvvv.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fanxiaobao.xyz/Article/details/glunmlilz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fanxiaobao.xyz/Article/details/gktzoofye.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuzzytgj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhsrgegr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsvmsfvb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fanxiaobao.xyz/Article/details/gybbsnypg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbvoznuo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gomimlkfa.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fanxiaobao.xyz/Article/details/gvwpppzbn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyrumqlp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwaobcah.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjoaohhm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyqaqxrxk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepxcqxwo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmdjkzrlx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fanxiaobao.xyz/Article/details/gatjvdxxi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuizkxkv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljedxmvs.sHtML

[D26] 数组转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gifgaoelg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gaehfxzte.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gmyxqewaj.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gipqfcbmz.sHtML

TS:   arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/ghyeskjyr.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gdpertbcu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjuxzhgx.sHtML

Ruby: arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gwtkdudtr.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgfvtvwh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfzjktkg.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkeypziw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/getgdeoyv.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gyaxfdcrl.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqgqtgzo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gahzyngtp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyknbssjz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gkxtrdsyl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyjpqzfu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gywlqdubu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fanxiaobao.xyz/Article/details/gahddytdd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmuceffq.sHtML

[E02] 重复字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gmkbqblon.sHtML

Py:   "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gyrybhrsk.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxielfovo.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/glfnuelpw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtjcyeve.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/geizdnzdj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjtwrvjt.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gdmggbwic.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gyhsnhphf.sHtML

[E03] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gwjkamtix.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gahxvidkd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfebavar.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gmochvrrp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpgzpeuc.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggabxcwoh.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gjepycxuu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyxkohnn.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ghcrmlfpp.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/guzhenytn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gxromdtan.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/gftosgcdy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/gzztsasgz.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbitehuk.sHtML

Java: s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfmucynq.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fanxiaobao.xyz/Article/details/glujaasyb.sHtML

Ruby: s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqzqesee.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gwydxknvg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gyvhkwosg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabrvqzzt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/guqgzxebt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlkoqxit.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gungpkmjs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/ggorrsbal.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunyppprn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsnaelzw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvctspaga.sHtML

[E06] 替换子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfczgloz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqwmbjtu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gknpqxxra.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/ghsntnyok.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnnulbnf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdphoxowo.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gequxqdaz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gwsvevqrf.sHtML


<!-- 参考信息 -->