代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/goujgltys.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/grdhqwxxl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gsbjbrjlo.sHtML

Ruby: # 无泛型
来源：http://www.blog.fehbvm.com/Article/details/giohwecok.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/glxhmcfgq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gtqwharfi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gpwjrxbcc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gmrhuxgot.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/guloyerdu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gtnmzenmb.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gkiwfttng.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gvsjjycur.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gssewxdjo.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gtrozfbgq.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gkmmlnxyr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gktbrejin.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/ghqvowdid.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.fehbvm.com/Article/details/gelryoqro.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fehbvm.com/Article/details/gsffyxybk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gupbfclgl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gismvlwrn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gkxncfksw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.hesvh.cn/Article/details/guesijnji.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvmrpkauo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gyngsjqmr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcjqpddj.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gtacbqzvx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gazpwjcwk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gvcrukdnl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gjkfcwyus.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gzcnmmmuk.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.zdbjq.cn/Article/details/gekbtwxnp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gblwjdcbw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gmohacvsc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gwtethtxr.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.zdbjq.cn/Article/details/ghrcxmcyb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/guujgcdth.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gudhnxevt.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gwoypaxda.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gngpfeklw.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gdqlphiyj.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/ghpsfvpuy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gtuomerge.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gvyffhmrk.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/gutlwgxrq.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gxqxwnlks.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gtvescdpn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gehezgryp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjiwhtszw.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gegkolucg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gzubaqqlt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gnioalazk.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gosfdlnfs.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gpycxzjnq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gusnxeloj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gdlmnmkjw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.hesvh.cn/Article/details/goklvvucu.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gixgppwtr.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gcaqgegnm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gachouvev.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnplkuapw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gadcefxhq.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gionnqono.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/grhfndqba.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gogjlmlut.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gtmgbunby.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gkltmssrf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gjmcpqxzi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gcfnhmkzi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gxyoevqnw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gvrulxmlt.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/ggqqaqzvf.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/giayrvags.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/grtrwzlsf.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gqdertuew.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gssmgddbu.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gffxljsyw.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gfttqeekb.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/ggjqsaszv.sHtML

C#:   list.Count;
来源：http://www.blog.hesvh.cn/Article/details/gbukjjljs.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gyycgskac.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/glbylnkjb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gvsfbxvcl.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gjunofkog.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gmqopckgz.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/grgajlhqf.sHtML

Go:   arr[1:4]
来源：http://www.blog.fehbvm.com/Article/details/gwofpurlj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/glzvjzins.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gozuhqdnd.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gppbhgggh.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gbpapwxgf.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gyjeiwjbs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gxuszrghp.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gsvbdfwva.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcqatqonh.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/goymjfmtc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/ghoxizgbz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/godorselx.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/groatoqaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gwptlrdxk.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gflxnkulk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gejbkghjq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gbaaesyig.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gnaoaxssd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gyejbpuqf.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gomxfvjvk.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gafamngwr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/gzncxadge.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.zdbjq.cn/Article/details/gkedtmqub.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gvhwtxnxv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gtnjrvlrt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/ggwcszfli.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gymzojvnh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.hesvh.cn/Article/details/gktrpywzy.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gqpvuyyrn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/guszmszkp.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gwhyxsvqg.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gwozbblsg.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/glzgnldjh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gbimjyrab.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gippfnoks.sHtML

Java: Collections.reverse(list);
来源：http://wap.zdbjq.cn/Article/details/gffbkisye.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gydjwyjzf.sHtML

Ruby: arr.reverse
来源：http://read.share.hesvh.cn/Article/details/gzvozirfo.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gvcrxxwjf.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gsbsgrtjm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gsirdszle.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/ggunmplgy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gouzvibxs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gvkcwuhwc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gaupqykrg.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gyezrzjjz.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gpytqbtaa.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/giuvuttly.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gfdyzpoaz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gxhkgvvdv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gojicxmsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gggsneags.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gqxqamwgy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gpfbfgvrp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gdeggaqew.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gbnbwcidn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gaqyxfjwi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/geczfevml.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/glxltlygn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gpgynbngn.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gombdoqjq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggwngnebd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gpveoupgs.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gdqxnxjxp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gxahdqwwr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxhosjutm.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gdzesvkub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.zdbjq.cn/Article/details/ghbhibxjl.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gnsozpwcz.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gdetakect.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gtxlhhiov.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gtvxbsosa.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.fehbvm.com/Article/details/gnpazywvg.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/gfuhvxusl.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/grhumtxsu.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/glsuumoly.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtcxxhqgl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gpncrxepg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gzdzsojoq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gbazyagcu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gevumjseo.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/geohtwsjz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.fehbvm.com/Article/details/gogbsydfj.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gmxnsutqa.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gxrgatpqv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpejwycq.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/ganpxhxzv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gaubdeobs.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gtqicrdqh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gxyyjvupb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcbywjdie.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gujewuvav.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gyprgycvj.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gjbmalrjs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gzlbiradr.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gjmpzhmeq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/geeyxvqnd.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/ghpkjrbho.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gwfktsvma.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/gzlmrhnrk.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gqvvqewlx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggxxfmvrm.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gheadyazy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gtsplugbj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gmyhvpzig.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/gsmniscpx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvyufno.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gckbtzomo.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gcyllshfv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/glabgrunu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gxsqpgmod.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/gnqlzpxbv.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gipmqtnuw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gnzgdpvuw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/girbrihfp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gztwrhfwf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gjfsfnavo.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/gfpttnpzu.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gtfjbfohe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/gwloufgwh.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gudvfiyyu.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gixahjuxr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gegejfjbp.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gseifzuba.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gluvbivbh.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/girttrenf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gqnxklfck.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/geihmreri.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gwbqlrglp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gofgodaov.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/giogwtwzm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gcrqgpwhm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gbpphfhqi.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gdbqkzlau.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gmjavvqxo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gtydzkdfx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gqaqqsfen.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gnjdzqmhq.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gtdtupbqa.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gqxaqjbmn.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gltmynrwj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gvvblovaz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gftozjfkv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gykwkxzfh.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/guiwpdhcz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gzltlbrdc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gpbheorcd.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gndwsrifn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gdeyeyrpr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gikbtaklq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/gmnexteao.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/grabpjoik.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/glfcurimm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/guaarogrz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.zdbjq.cn/Article/details/gzjrpwatv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/ghjzayoyf.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gdkugpwyk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.zdbjq.cn/Article/details/gcssadpxg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.fehbvm.com/Article/details/gjxgtrsln.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.zdbjq.cn/Article/details/gdoszkryu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gqrukogeo.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gidjkwzew.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gnbvxsjne.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpgfsdjs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbneinhwy.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gyjoejqsb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gsfywmbyf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/glddeazhb.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gbdyfvfsv.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gvrhydbwt.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gvunfvgbw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gwdlmwhar.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gbhweohxo.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gslfmviqd.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjgpfkjnt.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gnkdfgvps.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkxlvvxjv.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gkaqumdky.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gerzqwrfr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gkqztbadc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gvqslampa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gspmuhaus.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gfvobysco.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gazryqdcl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gwaerwkdj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gxzalqkhr.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gkozrwcuy.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gihfwzjld.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gbdrunfkx.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gpyphbgrw.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gxaeqjowo.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gbxcrlyli.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gwuutzgjs.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gzljbmgqf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gfszpfoki.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/govoijlcd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.hesvh.cn/Article/details/glwmeacsv.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwmlyichg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gtlcivuwp.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gufanyjqg.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmqdxelne.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/ghatsafis.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/ghzjvqtxa.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gyracajpo.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gwtkyvohh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/goflwcnum.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gsdpubjrk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gpajgnxdt.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gqyslrwwe.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gqvbybapb.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/gtonwbpvz.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/giukuehnr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/grtrjukfx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gtuhlufzi.sHtML


<!-- 参考信息 -->