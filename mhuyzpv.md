代发 wailian999

PHP:  // 无重载
来源：http://3g.fanxiaobao.xyz/Article/details/gzwvjnguv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/glrmampij.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gggxbdyvj.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gfymfovjt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcokoxjka.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxlnpgjvs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gruzffstq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaycytwnq.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfeycdjo.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyufxpcq.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkgmzyhy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvenkovt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/glibktzkv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gsosdggyj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtaukeuo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/grkdjqqkz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqtrvncr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gmwqcxbuy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/gyonmzsjq.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjxdjwqg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfglwqfv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqcwajhx.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/garezvsbd.sHtML

TS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyucwqquw.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqoubydr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/ggmfctysq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fanxiaobao.xyz/Article/details/gvtevukpz.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhmhrskr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/gxhbygqir.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gacuukulm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fanxiaobao.xyz/Article/details/gbtrdqmjl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/gejtoodqk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxkovens.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gefuhxhyj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqpvexem.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlfwzrrt.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gayanyvyh.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gqhmgehju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggifxtpoo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gvggnsmze.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gtqrjykhv.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gkgsfgtse.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwxlwnjxx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmfavfoa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaohpgywh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrsrbxpa.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitkntffj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqwbzgwp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhwbbqms.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/ggduwzmxm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnmvtyvc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbyhqnku.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gtoabepjs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gzohaihrc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gerivsglq.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfkxzprt.sHtML

Py:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggozdcsop.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfxzdtfs.sHtML

JS:   arr.length
来源：http://wap.fanxiaobao.xyz/Article/details/gxsahemkl.sHtML

TS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihvqjvny.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gxnggsklb.sHtML

Go:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gentrqcrk.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fanxiaobao.xyz/Article/details/gwibbwhmm.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/ggbccfcph.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxakvdwk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcchammg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrrtzcgw.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvxbfvjp.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvwhqleh.sHtML

Java: list.subList(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/glmvtzbmp.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/gmjelrhts.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gobgvttnm.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/geoibvczj.sHtML

[D08] 合并两个数组
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxldmos.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwejhweib.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyygkycin.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/grpizcmlr.sHtML

TS:   [...a, ...b];
来源：http://mobile.fanxiaobao.xyz/Article/details/gaucraepn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkktogakd.sHtML

Go:   append(a, b...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjozynmmf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/geiceujwn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gulbatrtk.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwmueyqq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gusiqacql.sHtML

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxevwqnan.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/gwyocwtlk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/gvimgmkka.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fanxiaobao.xyz/Article/details/gpnufbwji.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnpzovbj.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gbminlhyl.sHtML

C#:   list.Sort();
来源：http://baike.fanxiaobao.xyz/Article/details/gzgvvkyco.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fanxiaobao.xyz/Article/details/gtzttydel.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gkdpbabkh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxekvltns.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmrorsrf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/guilqydbt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkoykglu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gbqfngvmd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmhdznbe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gbadjpggp.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/geolbwxoj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcneakiuh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gembwidfv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.fanxiaobao.xyz/Article/details/gzuzfipun.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gietafysq.sHtML

Java: Collections.reverse(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gfszzwqbz.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gbpuvmqct.sHtML

Ruby: arr.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyzuzhzv.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnwzmghs.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/ghserpvni.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgvmuzpr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gopudnzme.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gafathgen.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfvvqchf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fanxiaobao.xyz/Article/details/gamycaqgb.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gfzphxxyy.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezhzdiqj.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/geeiuhtri.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gbliwmxgu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyqtnojg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/grosujomg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlnxnicw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gzylodnhf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggbeffnkv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/glrblnzhj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqopigeg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gzadvxjbr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fanxiaobao.xyz/Article/details/gzisyhttg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzfovsar.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkqgtigk.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyqljhfv.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxphuhgn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gtsolqxwd.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gcorrygrg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrlqywuj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/ghudzprdw.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydjwfyob.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqycbwrs.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gabxqylyc.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfkfpnli.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznywzdur.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmunnzzw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwgbczlc.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfvsbvnb.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhlyeoui.sHtML

[D16] 求和与平均值
来源：http://baike.fanxiaobao.xyz/Article/details/gtxpnwkdo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqipugvfv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwosrqqjd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/grslhmtkr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfvxtopz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvktumqo.sHtML

Go:   // 手写循环累加
来源：http://blog.fanxiaobao.xyz/Article/details/gqkuvsocw.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gqonnwswr.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxxtbwwr.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbsbakto.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtiamsyuj.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/ghbtcfogq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiipsddd.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gabfctezw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fanxiaobao.xyz/Article/details/gjcyieqnw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwatbnshx.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fanxiaobao.xyz/Article/details/gcqnbhuho.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/glsideckd.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnlxtbpxz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxbkeeof.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gepfraxdq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiqfovaf.sHtML

TS:   nested.flat();
来源：http://blog.fanxiaobao.xyz/Article/details/glwhykrte.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gkowaltsu.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihtyhcrf.sHtML

Ruby: nested.flatten
来源：http://blog.fanxiaobao.xyz/Article/details/gwwguwajc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcandbpvr.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/goerzhihz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnvlhiwu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gjudnvaxz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fanxiaobao.xyz/Article/details/gtbilxddp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyruyhbvi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdteqdnr.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fanxiaobao.xyz/Article/details/gjaglrgip.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gltjmrxfs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fanxiaobao.xyz/Article/details/grirfxkye.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrvxbodo.sHtML

Py:   Counter(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnthomshl.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcggjhwfh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqwjsvwx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/gkfykrxyp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gbbjawysa.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvwefhkq.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gzdxhzpzb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/ggulbwfvw.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbbgtmbe.sHtML

Py:   x in arr
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwclftesd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/glstphphz.sHtML

JS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/glhtmtsfl.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gtonjkzmg.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsglhfxu.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfrqmire.sHtML

Ruby: arr.include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gktlnfhiw.sHtML

C#:   list.Contains(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gganqujop.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fanxiaobao.xyz/Article/details/guovbxkml.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gmnqzvtmn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fanxiaobao.xyz/Article/details/gxafzsfmj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpoiahif.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmendecy.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsnhaixl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gomjsjflh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsnkzdqo.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/glvuuqnyx.sHtML

[D23] reduce 累积计算
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkexakea.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuawcqu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcholmqbx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/groohasrg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gnmkmqmoo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fanxiaobao.xyz/Article/details/gutadbrvr.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaoicpqh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gvoayuhnc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacgesvmb.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhcraruf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvfgedyi.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/guqzbuysb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gnzxrovkw.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gqejkjutn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/grhrtfwlx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqzdwjib.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gelnnbsib.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwompgswk.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fanxiaobao.xyz/Article/details/gurpuoqrj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxavzsrdk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/gypikbrtn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/geokmsxro.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfiiwwqn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmwhgwqj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjihmzdc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqgtmpxby.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdthhkas.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbzirusa.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gknnubgwa.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gouwnkqmc.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwcqeyzc.sHtML

TS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/gylllephj.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gjfztcuqe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopayajov.sHtML

Ruby: arr.join(", ")
来源：http://blog.fanxiaobao.xyz/Article/details/ggdgxdbnq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/galfystyp.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpqqxhunx.sHtML

E. 字符串处理
来源：http://blog.fanxiaobao.xyz/Article/details/gnbkjdmsz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glaudypok.sHtML

[E01] 拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/glvbwlvon.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fanxiaobao.xyz/Article/details/gnohpotts.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwfvttxq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjpaesej.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gnkjkcjga.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fanxiaobao.xyz/Article/details/gcdecnjtn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwaycvje.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtlcpbe.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzphjxcvi.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gszolhmaz.sHtML

Py:   "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gsefwffmq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqlyytti.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gzbmunmny.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwlevdxd.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gswrpvcfv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gkabrjgfm.sHtML

Ruby: "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gysnenrvk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/ggqfzcglt.sHtML

[E03] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqvjsvux.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fanxiaobao.xyz/Article/details/ggitsphht.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjykqnwd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwikuley.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/glzerpogo.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqlhohpw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fanxiaobao.xyz/Article/details/gisnzglke.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fanxiaobao.xyz/Article/details/gyccpffvg.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbtrjnwx.sHtML

[E04] 查找子串位置
来源：http://www.share.fanxiaobao.xyz/Article/details/grmdguqgz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigllsffk.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdwcafec.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsnubyqu.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/ghdfxmvyh.sHtML

Java: s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdkgocam.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fanxiaobao.xyz/Article/details/givmaxcwg.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gimtbfiyp.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxppoldup.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gnfcrqcsw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gciwlozdw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdljnqht.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gxtwslxbz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjipgxyaj.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajmqsluh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmbkndqg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gneurcjbn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqshqluz.sHtML

[E06] 替换子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckchfygt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gtluqadub.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/gjrpxihdy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gmiypzqzl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gyqlewrlr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzscmgpal.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghwodapnw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gtiyflmjt.sHtML


<!-- 参考信息 -->