代发 wailian999

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2itvdsjrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rxzckvvi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zhelpkpd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2otdqnxcd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nhmtgzfr.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2tvoshtcx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mtxdxkpe.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bjkhurxs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xabhytfx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2smikkdji.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kvigapuj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fffbivgy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lpyjfwie.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nwxvumbe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ybcpudub.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2twczuyqf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dipgtdnw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2znkplwvd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sbgmonkj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2wjpzzxjc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kiivvbyi.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uyrzparj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2injyttwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjmykjvu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2leirgies.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdxvxmrb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sjjxmzjz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2irnzxwab.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lnhtptto.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzekjkkp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ltrvhglb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2saozvjup.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2rktczqmi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2noklfpgp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2sowqmptr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2emdkxwnh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2rqaitply.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jriltuqo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2renkrtia.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hwnxzirx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vbiscghs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2igoavchf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2cnybhhgh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2aqrndovq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2rsznfgxx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ufmnbdhh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rruyyyfu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hlpqllxy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cqponqpf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2iinatyvi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lerxtwml.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2eqlfcarr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zuhrardj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aglaqmen.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pwqtdkjk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvyullun.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2tsjvfvsx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oehoqyvi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aguszwtk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sorqtued.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lsgdlxxk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2iplvbpfc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gzrxqzaa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pqlwwoqc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hfweyyld.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2djohmvab.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tiiggziw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2uwfmejqv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wutsyfyz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xhbsqrbn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rzkjiatu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tvqumoxb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2imqanmzu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mlbsinez.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2khrybzqi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2huyhosvp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jpunyfad.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kiravjvz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vxwwlxmr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2mherdfjx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2nxjqvexq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2bfgojhmz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aflqohlv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wzsjfhtk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cztsgcgj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2txgorsts.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xiuieziz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2windngxw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbvhylpa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2mkvjasmn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzekdvix.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2plfgrewj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jepzwkuu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ldhcwadm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmcvvzs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ntleoxtl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ksbuofzw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqxjnegu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2guqodqnp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gowakhet.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pedcingk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wnuljfwe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xvpabooc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ncnrotno.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftsnrcoo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ebqdverb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vasmtqbh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2iaxxnzgg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmfoqsa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2uvhdvaco.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmftkrq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mbfeyrmd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2iaarxunn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ivvvnqoy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2tftjhdqd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2afcnixcp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2iwcfyjlb.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xuyxzelx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2fsgnlcnk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2qtukfxmq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2obcpolwd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2lunfjrlz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2xphlkbum.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2exkcarxc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zxuodxfa.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xegugyom.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2iipxhvla.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2hcpnjvix.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2fuiwxgsn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2limpreab.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mnpduhlv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fnbrxxbx.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2cvkhpsgp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2qzwkodpz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wkotqgtt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2nplnnhqp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2navxhgnq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zuwohqny.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2odipywct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2inxsbgbh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2gdegyxif.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wgtcykle.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2neokxzog.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yenolztb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xrdvghip.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2mvdjqpib.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2filjsxou.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2irckphze.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cbdnbdwt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xifpkfcq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtbplnez.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zmuiblli.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fvmikfxx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hpgriyzm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jblipcxt.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jqtlwdac.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kdrxqwao.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zdnplamf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2sjjivmjv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kvyiikiu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2acvvgzof.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2shmhbjaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ghlbzpur.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hsdzendo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jsxmhohf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tdjkjkvz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ohxcgqkd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2fkrxipur.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wntmhvjq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2yraigjpo.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2qaemmneg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmgxvpxu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ryrtgwem.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2pjtrfpfq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2xywsyyud.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qsirqexf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tueuahrt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2shezetjp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2geaskxhs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2licovpsx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2egvkbpil.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nvizalam.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2gvntqonx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2hwayhnwk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2biqohcgl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ofjughzw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2alubcrdz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wcousxie.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2lnztsypb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdpmbckh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2vjxvwsyj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2talvzjob.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2cykgdtre.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2maremtra.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2hrpbqcrm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2jvbnvbgi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2wrvygzob.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dkyryfvq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycvbwkdg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pvpywkvv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2aniahhmd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2morwwyxj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2ntveiril.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2obqvtmmf.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vunfmmcb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2svkidlrv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jbomfvnc.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2djyfpdqy.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2eqrzvldj.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cdviltkl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edxbzrtb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sapaztet.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocdopiqv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uregyjkc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qnhjanyz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ihxqooaq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwobrfnp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2pnptbcco.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcglsyy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2piuimrsa.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ktkgybeb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2zddfviip.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2lyfaaevl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2nblguhhj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2suxmfqnm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2glvbqard.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2okczdlmp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lisjcjfj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xbavwpff.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2azgcdiiw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yckwurtd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2aagvfsfj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2dkolngvg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ijvsetsr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ihqasvhj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tjbuqrfm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2tiajhbba.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2aahvnofh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gydvxgqa.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yzbjjlaq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vmjmavdf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rcerhzpm.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ixumedtg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2vmcwdvmq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2bqnourub.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssjezgfe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2widwbnvu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mieemngr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uffovylc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hscffobg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucdktaog.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ryrcurax.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2awhmhoup.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xpgyfern.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gfafxumk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2itwlkekv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bxlhemxk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gbjuomjo.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mbmzwjlr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gqrntyft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niltwmaj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2keytzvrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nggiklmb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qznzmjuu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ppawfabm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2himtowlj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2irraehbb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jpdbqvxy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jubgaoab.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2juifiedk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2azoqduee.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gbvybnko.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kxogupoh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vkeixjkx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ipilvgjk.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2scyevasf.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnbypye.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebezibkv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwvegurv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ozhfruzt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xspwezqa.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ztrfeicj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2qjjlnfxr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2imheyuie.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jqlgkfse.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvnispbs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ianyxlyy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2smibyxqj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2njiqugnt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xlyvqbog.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2biqilhxc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fgvqanat.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2elwoggwg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2zkiygcnb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lfhqradl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmwryi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2zyukkgnj.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lakcyppn.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kfsthxlf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2folinocm.html


<!-- 参考信息 -->