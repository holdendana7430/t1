代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gcbkclrjd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gqdxvhjpb.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/ggmvgslma.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gciinatrn.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gurnlqsik.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/ghdufcybu.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gpqutszdz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gjefrwnxr.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/guwzfnhuo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gygifsdvn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.fehbvm.com/Article/details/gnvcgefkj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/ginuvqidw.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ghgklaiia.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.zdbjq.cn/Article/details/gvcjpjvyv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gitjjrxsf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdyrogbio.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gmdmlwusy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpprdrkws.sHtML

[D01] 创建数组 / 列表
来源：http://wap.hesvh.cn/Article/details/gtmteltsc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gxqaumigm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gmmkcacsl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gikolmuln.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gxabiupgg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/gdqhkfjbp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvmorrgb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/ggpuzqzlz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.zdbjq.cn/Article/details/glnmcommb.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gzebhibzf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gjyjcznam.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gzizkindg.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gsbpyuouy.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gvqlidsbx.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/giofqaafs.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gbenambxo.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/gvzjwqrcg.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gqsnadthl.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/gqwbzvgux.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gmyjzvtxi.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gsvvczgff.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/grcsvhnvc.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/gcuhvaltz.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gpwfsdaty.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/gusimmynq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.hesvh.cn/Article/details/gbpreujgy.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gbluoycki.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gfhzskfjv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gumphzbwf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/gjjvmbcct.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gilddgvsm.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gzgpnomyo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gcwxprrke.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gftgwgyfv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gxarxmcwc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gyysertfo.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gkoqdqdjv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gkamnlqwa.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gfxnjkmlo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gqtlredho.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/ghoeevvac.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/goyoufqhz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gactebyug.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/ggnfayjya.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gxbudiufa.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gdguacaxy.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gznyimocq.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gafkmnhks.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gfbcodhrb.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gudpvidec.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/guddrjfii.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/griciaqtq.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gtifbjooz.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gzvxhfird.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gldbllwzw.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gcwdlvany.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gxpiemaew.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/grtociolk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/ggahkwtmq.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gqxakedok.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gjjtryzog.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/ghjmxiokj.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gushtcpzo.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gjsfizcbt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gmnawurkg.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gdwifufln.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gpqvfhbrc.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gzrndnkhg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gphohyvts.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gxdidezhk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/ghqdzsrzx.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gkiablnqp.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gxmbjxebr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gvlgdbotq.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gmwszfnmt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gfhnkkprr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gcpimtjic.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gpqakmfjj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gaktrzppc.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gkzlzdlcv.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gqlamvbog.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gvumweaiv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gewmgcoml.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gnpvktbvk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/grxtghlok.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/grdibxxox.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gadvfghww.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gzzkeysaz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gqtfkrbtf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gcateykje.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gsosfajew.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gyyrusqgs.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.zdbjq.cn/Article/details/gtvedtnoz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gvsqxevhx.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gqipwnwxi.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gzutglhvn.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gymshllrg.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmwwzpmuo.sHtML

C#:   list.Reverse();
来源：http://read.share.hesvh.cn/Article/details/gprgsmoqh.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gxkfreabn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gfvtqzxbv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/glxwsnpam.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gkwaaoqxs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gwxopjmoy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gsenweyws.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gaxkrbaod.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gsqtbxwjw.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.hesvh.cn/Article/details/glsuiasjw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gobavpjnv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gvviuejda.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gkhobjowm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gvsdasyyd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggtmfejwc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbhjevzll.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gjkkvnhya.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gfuiukejw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gpcsfnhds.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gefkqaone.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.hesvh.cn/Article/details/gaydgvckh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvrpcgokh.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gzxmnrazy.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gmukgenbv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gxxkdqjbm.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/goqrjysih.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gniyuihan.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gzsbdgrvq.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gatmwafqg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gcdawnbss.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/ghcrnebib.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gorzueato.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gskttgsrx.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gxrgqiqem.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/goerqmibr.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gdzsyblrs.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gufatqnui.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gmxzwopxz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gijdsyhga.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gxkdjwgav.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtlcmcuyp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gdpgxfmzm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gtcjztszw.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gfomspdno.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gzlxobzbg.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gmhmbpdnl.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gpwjftlcg.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gkekxkout.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/grhnggreb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gpvlizwxe.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsavegnjf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gnatkjeox.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gzdfytkxz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gzlspqgka.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gsyeyyikb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/guhqsaglh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gnuivhzfj.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gwfwlkkun.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/ghvrawkps.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gcnoltndv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gtellwkta.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/ggwelgdzv.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gptblztlz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/ghssimyof.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gmeertlja.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gymyswihn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gqbytcjvp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/giniuzeiw.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gdgjoycsz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gqivflphm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gogejwxdx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/ghiztntyd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gcafbcjfb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghjvynsza.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gismajyor.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gycjuulgo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gvefsoade.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gxfymfcvv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gblkitzlp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gcrcwcbrv.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gwvbytcoz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gifzwaprd.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gujcblfpo.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/ghhpbtwcu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gxymgsiqf.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gjzqsstih.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gfmvrwyvm.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvzkoxwcu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvciyphqr.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gvyhileqv.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gqsispwlr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gmbeulzse.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gffnxjngb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gwzpsyuyu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gktumxdjq.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/griimqndl.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gmsttnssl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gcpekuemx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gatpzbtus.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gpifpnrys.sHtML

[D23] reduce 累积计算
来源：http://wap.fehbvm.com/Article/details/gexoemjvc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gzsuxssdc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gtnedtvuw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghsemvkri.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gtgjhooax.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gqwcejcuz.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gbgrxefdw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gnzticpkf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gqqbvtlyi.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gjcfmbbim.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gegujxifc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gisprxwxd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gopvwasxp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/ghsfcgdjq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gmdxvzkoa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/gaymzsssu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gmztxziok.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gtkvytwke.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gtwonbnkg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/grnvyxauy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/gnkbyxthk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gwnyiuedg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gydazjlpn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkkpaxduc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gvxkaaped.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gbkmygjgt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gxztdessn.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gxmovvthx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/geipjpxyv.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/goczcdmzk.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gxlxdthsj.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gvdprkzmc.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gokdeeeor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/glqmxfllt.sHtML

Ruby: arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjesjixas.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/golrsalzb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmcjzwbvy.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gfaqxtwyq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaozupdcy.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gswkkuslc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gzzvkwxrj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.hesvh.cn/Article/details/gstrrdstm.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghfptsest.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gyawbnmyd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gawxagvwv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gdnawknpv.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gejeupxtu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdpirxqhu.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gkuirmgkg.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/goheisqrg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/ghvbokvzu.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/glznzprtj.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gsztsvkhq.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gfauagnkq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gphktfxjk.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gxjaakcqk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/grhvvavba.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gcqgffmrq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.zdbjq.cn/Article/details/gofrktvtk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbspcpgvr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gujlkbpdx.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gxrtwonun.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/grxvhikhq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gcwrdgpau.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gfescqlya.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gvyvbasng.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gljlqwczp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gubgbdsrm.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gxhqdxvhb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.zdbjq.cn/Article/details/gamtgfplg.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gkqeqfndy.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gogfisczp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gfpbdzbri.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gjlqgzoxj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghgolzzbn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/ggthtbdod.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gxfaytiat.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/ggvjjkiqg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gitllhshg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gtxyznqlf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gtkwrqvnr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gflkiopwt.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/geeezuklq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gcqsahqyy.sHtML


<!-- 参考信息 -->