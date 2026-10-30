代发 wailian999

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrnklzbv.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeknazha.sHtML

Java: // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/getjzfkdj.sHtML

Go:   // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/gjvtjdago.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gejsfxqmm.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcstzzix.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gweylpkhs.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fanxiaobao.xyz/Article/details/grpjnrvpp.sHtML

PHP:  // 无重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxjyxeku.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gantrgpow.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gilkzqmro.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzohrcvxp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmvvuxmx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlxmegso.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhrnlblz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlrlrpcc.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fanxiaobao.xyz/Article/details/giqjivsnf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gpqhvjjgg.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsikkzsnk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grflkgpkq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gpksmkihs.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/gzpdbpupu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fanxiaobao.xyz/Article/details/gyhrernps.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnqzdqmq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwkcshvc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gbmiebwxs.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fanxiaobao.xyz/Article/details/gfszppvwg.sHtML

[D02] 追加元素到末尾
来源：http://blog.fanxiaobao.xyz/Article/details/gbmdlungk.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpozrbieq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryetmypn.sHtML

JS:   arr.push(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpyszjbmc.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpxhwpaw.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhcqlhxx.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gshfmbkia.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fanxiaobao.xyz/Article/details/gxhbafndp.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnycaszrv.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gctoskkeb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyebnglqs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxmjgcgl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsqhtfzf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuucloeh.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gzpqmbtgj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/grbyvfrod.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.fanxiaobao.xyz/Article/details/gdiavizrh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gqtixyvsj.sHtML

[D04] 删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/getksrxty.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzuzdtzf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcoxfqaq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gtsdctqfi.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkypejeoj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gahybbysk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/gjowepwzj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gwzxhyfxy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gamxrwwyp.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/ginrzhiuc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhzziqgc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnadihobc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gocouquuv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubroakjq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzfpxaqb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqfvgroj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/guouveonk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/geqhqyxkl.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzzgvchl.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuihmerk.sHtML

PHP:  count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/giiafulcr.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grjoeudhg.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gitwbjqxz.sHtML

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbvcvtao.sHtML

Go:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmimkoigh.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gbuppvead.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/gxlbythkr.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzcrdikb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fanxiaobao.xyz/Article/details/guebupasn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gaujocsad.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/giukpdrmv.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqjamdli.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfzurihpf.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnvswqxf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugexhlum.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwrdhjvoh.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/godcxqrqc.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrjjvoso.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fanxiaobao.xyz/Article/details/gurupecuj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.fanxiaobao.xyz/Article/details/ggdabmzkf.sHtML

TS:   [...a, ...b];
来源：http://blog.fanxiaobao.xyz/Article/details/gxltnccvh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/glsozcxvw.sHtML

Go:   append(a, b...)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfretxjn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbshlchia.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwxxqwvx.sHtML

[D09] 排序（升序）
来源：http://mobile.fanxiaobao.xyz/Article/details/genyyqhnr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gdygqoros.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfejtcjdr.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gbugyxbtr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fanxiaobao.xyz/Article/details/gelcbuyxy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fanxiaobao.xyz/Article/details/gykumtcry.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gckyiyepw.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgfdzlcp.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpdzcuol.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/guumfhvej.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjccewinf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gorunzicl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gywoffsoz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjbkmvnm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gaunimfcy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyagnlot.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvppcvlem.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/glooyfqol.sHtML

[D11] 反转数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpxkyouq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpkxqppq.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasftdlno.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjixcyvo.sHtML

TS:   [...arr].reverse();
来源：http://wap.fanxiaobao.xyz/Article/details/gpuweqkpr.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrfvykjt.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtyjgqck.sHtML

Ruby: arr.reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gogtoltim.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gvnppjjsk.sHtML

[D12] 查找元素下标
来源：http://wap.fanxiaobao.xyz/Article/details/ggurzsrsk.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gfxhktjhl.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gasjdpwde.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gsoncvoug.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbazbdtm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fanxiaobao.xyz/Article/details/gwumfvvas.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhtkvsak.sHtML

Ruby: arr.index(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcfbdpyo.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fanxiaobao.xyz/Article/details/glvtxbtby.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbfocdrt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gfdqiwcck.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbislggr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrpnrdqx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgvrklgz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjprmvaqk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybxrvnuu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdqhfbvx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyspnitu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrgxolui.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhncsfhw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/genlokrzm.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdguapwi.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gglbgrhqx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnuejqia.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gudvnvlit.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gaxivzxgf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gkatxcizw.sHtML

[D15] 去重
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaolrgfk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpcxirwb.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqazereks.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfloqcsow.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymiosuww.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpllgabiz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqntxrie.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrbjkqqb.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/grcbbsyxf.sHtML

[D16] 求和与平均值
来源：http://www.share.fanxiaobao.xyz/Article/details/galfqjpud.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybwkxdev.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gxqpxnuoz.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gluvwosrh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gxmocyvqm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxxhtjjd.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbcrdqlt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gkxjvsecj.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsivmzqqa.sHtML

[D17] 最大值与最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gknborjcq.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjedjkbcl.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxtmuxdk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gfybnjiyd.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gymnzacmv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gvmdkysjv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gaufaseib.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrvoqexb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkusokygz.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkndeupl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fanxiaobao.xyz/Article/details/gdehcabtx.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnamhimz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabcpupod.sHtML

TS:   nested.flat();
来源：http://baike.fanxiaobao.xyz/Article/details/giktnepct.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbucjksur.sHtML

Go:   // 手写双层循环
来源：http://baike.fanxiaobao.xyz/Article/details/gkugvrndd.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gvagnjwwy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpfzrace.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqppenoc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/golxncxbq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjazvbia.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fanxiaobao.xyz/Article/details/gxvkkponr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fanxiaobao.xyz/Article/details/guafiwnpz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtonvcltf.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gdtlawraa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fanxiaobao.xyz/Article/details/gdvtsxwlq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/geciolfkd.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/gerhlctux.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcstugnm.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhmnmfmg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzurhnac.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/giiavjufi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigfdmiwe.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqzvmxcw.sHtML

Ruby: arr.tally
来源：http://baike.fanxiaobao.xyz/Article/details/gqyrwnfvp.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gritxethw.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsiauxvv.sHtML

Py:   x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyipizhh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqtioypd.sHtML

JS:   arr.includes(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gycbzqgay.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gyjyxozbc.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdinwupef.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkirlehnu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrjykzho.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gespbalpd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyixjvkfm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgvggfxu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gilqtbols.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzopeqb.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxbawdot.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfihmwoc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gockwgoxq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fanxiaobao.xyz/Article/details/gkkluxqhm.sHtML

C#:   new List<int>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfcblyngd.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gfjhitgmx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvtaoeic.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gprlrcduh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjycdijv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcgilgmz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/goovbhexb.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkajiqoo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fanxiaobao.xyz/Article/details/gftnigngk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzbjwvac.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gpwzdusco.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuqoyhqb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/giisntvym.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghszubydd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwuzoyeb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gtdhnghuj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfjlyatl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/glnmsojpb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fanxiaobao.xyz/Article/details/gktrhkcxg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdelvdptm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fanxiaobao.xyz/Article/details/gwzmluazx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwamxemxt.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelxtqnik.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gznmjekrz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwfubtfkx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeqoqccc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gedjwqhnf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwrtetuo.sHtML

[D26] 数组转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gxsnekycn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gtkuuggxy.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmilglwk.sHtML

JS:   arr.join(", ")
来源：http://baike.fanxiaobao.xyz/Article/details/guthqkzaz.sHtML

TS:   arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gshcqykru.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpkhtxvk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gfpmeswdw.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspwwkoaz.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdolzrj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpusisxkc.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbyuonfq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhaukuoa.sHtML

[E01] 拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiseefrn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzxvviwr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxbfempw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gbjvrfubu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxrctxhj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfaohhezk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fanxiaobao.xyz/Article/details/grilzjvcw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmzcyepp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gtdoifenw.sHtML

[E02] 重复字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ghdiwgylw.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfsvpoqp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsdevujq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/goyocmmna.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtazceikg.sHtML

Java: "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/grwmxwube.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gjzdkmgqj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbzocnr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.fanxiaobao.xyz/Article/details/grcaljnro.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxngrceez.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpitlvnzz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gfmcnhxon.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/grnatmpnu.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gmbclcqkz.sHtML

Java: s.substring(1, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gdrcofbdy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbqfmssf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fanxiaobao.xyz/Article/details/golvfjege.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gkqlkajho.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmrljtau.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidgsasru.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtqmqgs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fanxiaobao.xyz/Article/details/grcjfcuyp.sHtML

TS:   s.indexOf("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gotpeuden.sHtML

Java: s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfgqhlvm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghnfnmfrm.sHtML

Ruby: s.index("x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyuymlgzt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufrgmevu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gbmmwuuxb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrekrqcv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fanxiaobao.xyz/Article/details/gkplpzndg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvbrgqux.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gszvpbepp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fanxiaobao.xyz/Article/details/gckuctspq.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gobrtumyf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gwgwutfmj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/guleztqhf.sHtML


<!-- 参考信息 -->