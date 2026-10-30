代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gvfmfzlha.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gnatlxcjp.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/giakurdll.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gwwxxiwhq.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gwagcypgo.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gvvarqxmi.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/ghyocsvtd.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gnndgexvq.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gsmlwehpn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gsbixafhx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gnirksgvh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.hesvh.cn/Article/details/gwxzceatp.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/giqxccbtv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gggpmiwdb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gxsffyezh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxxfnhzqo.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gffcruezx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvvilvcja.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/geiggyxvr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gbyuytonf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gocrxkayl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gckfddtzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gbmglzyuj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gidopiceo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.hesvh.cn/Article/details/gqfkkgkpi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.fehbvm.com/Article/details/gdvhmpcdx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/ggndeghff.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/ghyfqtuxe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gjpflxvvs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/guixfsthx.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gosmexkab.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gqbnrngum.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gxmjznfzx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gzcivwuuf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gmzlmfcwv.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gegahjhtu.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.fehbvm.com/Article/details/gkphtkuja.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gwmccsnmi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gmqbehjkl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gmeujqfgw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gloeaheke.sHtML

Java: list.add(0, 0);
来源：http://baike.hesvh.cn/Article/details/gztdajcsu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gemqbkhjm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gahqcyumf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gajuudbou.sHtML

[D04] 删除元素
来源：http://wap.fehbvm.com/Article/details/gtdtfepjo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gpnlfcclt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfnieapyh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/gykacvxzr.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gbihwqnmx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gaksvdnfd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gkronlual.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/gvaisxykc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gpekiqvfg.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gtpetgwje.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gaehvqeje.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/glkylxrtj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gighjamew.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gazhqbbif.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fehbvm.com/Article/details/gugvhaigp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gpufwmyyy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gtzyjuyri.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gkqdmygnd.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gwrxbtdwa.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gjhfmsfrs.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gakzanfpl.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gewmgdbyy.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjaljgzyt.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gkqnqcxzi.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gfxofyiek.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gskebyddi.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gvdieftfo.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gyyeppded.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.hesvh.cn/Article/details/gxlxauaku.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwisdspag.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gkdbmjsmd.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gbeiydwae.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gdyuerued.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/getydtptj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gwmdimcxw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvgdxbqom.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gsgcqmtje.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gtbtkpiql.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gjvjfcyzg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gdovuyucg.sHtML

TS:   [...a, ...b];
来源：http://www.blog.zdbjq.cn/Article/details/giuujlouk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gelvaorqu.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/gxbytlqvx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gunqvzadz.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gwbfbzbgh.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gthyipmnt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gzmajuxga.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gixkuntyc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gsayukclj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gwzvyixhy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gchztgubo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gripsmkml.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gmyyhuuhs.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gxnvpfjau.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gakwbcsda.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.zdbjq.cn/Article/details/gbxhmgrxd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmcgurodf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gpqkodobd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gkomqxbzi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gqjxnfyib.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gbufeoewg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gmwakalfb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/glqgnpupd.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/ggithrpgq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gnfrexilc.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gvbufnzcu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gztrnkbox.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gcvvyvnab.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gkpvitmxl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gjwnimsna.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/grgjvbvig.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ggwolbvde.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/ghggwiqyf.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gkcmuyfud.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gprlhoncj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gyodazuow.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gmniszcew.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/gizkexpwi.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gcwdyejyl.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gfvplouow.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gsrvwccjn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/glbnlqebt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gaowhahop.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gyqlarwju.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gbziplxul.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gngxdgtbl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gvcqeprwk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fehbvm.com/Article/details/guniicusw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gmifvmqku.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkanqsmdj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/giyhrsqdl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gawlxyzak.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gblmdjbda.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gjisrfnjg.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gwvrrjntf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gccbxdlfh.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gcsgpmhpb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gyxjfnilo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gvshipuuk.sHtML

[D15] 去重
来源：http://baike.fehbvm.com/Article/details/gxvdsjomx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gtgdtzsax.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/ggbmjgmqh.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gqnyqrmgs.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gicaqtpnf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/glqupywyp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gmlcoytdz.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gnrtekfzt.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gmotdzwmv.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gdymrkkuk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gscpzvpjy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gizyjapzw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdpetlrcq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gkkofsrzj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.hesvh.cn/Article/details/gvifwlmkg.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/ghrvowehq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gbkrvnvxn.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gmrpytpcx.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gzcmjozkc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gwpllmhbk.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.zdbjq.cn/Article/details/gqrydjdue.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gwkzngkte.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gotcyphpe.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gvlwecasn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gkxsiocbp.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gxdexpzaw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gnbmmxyiu.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gapyuflyn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gzhzggkeh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gqpjnbgfi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/godzztnji.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gjscnsgpg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.hesvh.cn/Article/details/gznueayup.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gnkujtwht.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/grfxngnxm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gavjlybty.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gfseweine.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzyymjvf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gslabqsrc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gyvlwbawq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gktmlwpjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gqdxhpsbp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gvlxyqxcn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gpjasbwoh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gqrrynuaq.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/grucyxiqh.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gdnhqigao.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gkdzbjqns.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/grtfbjshu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gdyfcxkkv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/gjztluxyk.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/guznedujp.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gvnjqnemw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gfialhdsp.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gytzhwbzf.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gbpxevgve.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gyuxdnahu.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gjcnzqwpy.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/geuhvhmnh.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnekjyscw.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glbsvbbft.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gwrrbjhwu.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbcjoxrod.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gdqqlnxil.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gusylxvcd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gcvarwcou.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/glvpwkwtc.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gubfqhwrj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gnrkutdgj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gyplqyudt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gqixeaapt.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gikcxnmqd.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/ghquzdvcw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gtiwuocnc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/gydxxdhgb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gdatwdaam.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gjnuuwypc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gzhnbngqu.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gtxxqqfep.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gpcequxos.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/grdqyxvml.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gmnlfkqxt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gxoyjprke.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gljasbwvp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/glfvymhku.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gsunibemc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjgcrgohi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gtaqhgbjq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gzdaftmxz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gahnxxnvy.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/gpvgphfiz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gekouulvx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/grvdfpfga.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gqsiqtsno.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/giltbpixl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/glzpnexkj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gkhfajbiu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gwhdokqwy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gfrkpfmnq.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gzusszkzu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gnixzlnvc.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gexcvstio.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gjoadpsrc.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/giuicknzc.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpyenpkyt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gfawtmbjp.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/ganqnekln.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gvrvfsesg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gszufcujz.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gyhzylxkv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gczaieraa.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gelpgtkdh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gwvoigxep.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gtdlhdjpv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gmbsiwzmo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gmjkdivtq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/glayfmjwc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gltqlmzdt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gsgfluosf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ghyljbpiz.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gnhrqhqsr.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gcowwauxv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gtkmcucut.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gljjjvkjf.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gezagnckn.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gggqrzjmg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gggxtstag.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gxjnbqqtz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fehbvm.com/Article/details/gmhcsqght.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ggjggaigi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gadinenhk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/ghtfzriac.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjwtmqhek.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gciscsiwj.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/godpnfdjy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gduhtuver.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gvmciczid.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gvtznazna.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gmytntrnh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gufmfmxwp.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gqnmnhkyd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gkqaubvgu.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gloackvff.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gxzgqppop.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/goaqqcmcg.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gmhqaeaib.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/giogppzxl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gksmmxnqk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbyhcjkc.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gkfeukqgw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gfylkhsnt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.hesvh.cn/Article/details/gblwgnnzj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gvogjawyt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gwbufdbrs.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fehbvm.com/Article/details/gnmwkbqzt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gqjxhhfbv.sHtML


<!-- 参考信息 -->