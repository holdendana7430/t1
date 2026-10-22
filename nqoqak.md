代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pbwwwibq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2yirwxfmz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rxhjmtiu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dcjcqcoy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdrqybii.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjbvowsb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2fknwwcxl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sqkpfack.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jaeyjzca.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zlfcrsmc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2xnhbdsja.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kzjwvyir.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yjaxtnmz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2unigvuqj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ushmofty.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2afyyncci.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mudgeddm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oaiwpbyc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kjnlilgc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fklwdeki.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2cycvhvut.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ypahmhwv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2bmdkgacg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlgkiolu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jbmeacto.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cutqhbhb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2enbxadeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obbjaxbb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2jtqckmkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yctrlmld.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fjeemlek.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2xgdnvntc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xedwdpro.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dckrbipu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ircismbv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2cpwittgy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2mucoaavj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2plxkjqbl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2pwyyofwx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hhegdkso.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gcnfcazh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2burwuqjl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fyxunpxd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cooaxozr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2kdihjpop.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hepzezsc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbhsgwx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dranjovt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2adzrzexn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vfutvywa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lpvugxlv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hffknupo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qvsvnsqk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vxjvupfq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hevawvjn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2pigwnblh.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2amjbeyxq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zqxhylbh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2llfkmujn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qoagmtlz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vdnxzoke.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2mcthiqgs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2swfhonat.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kvcbokrf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttkxwzwr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cdztuxrd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nxvwtxhg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lsbwlwnm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xkzthlsy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zetqgibh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mmedfpgi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2intvfsmb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wxptautm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wutpakfi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gkjapgwp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sdwblipc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nbnvzezl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wvuofeln.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2juamznyy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pupipdcm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ypoxqejv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfptxuwz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gtiifszj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jtjlcdyc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2rcrymvri.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jiljfprm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2thgvtekg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uhhlbxzk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2akgefumj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lqifzlft.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2phjxumtl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ddedyzij.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vskhxazu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lwdxmjbn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ejpnrivs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jmdzfalj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ecyvtgjp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2icauygkj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfmixddb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2aerxhmgc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbknrvf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cbllqdgp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dupwzgmq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2udyaecab.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2hjcstpdl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2opjbesja.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pahiudtp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2tykcdauc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2privcedc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hslvfxpu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kubgqcnw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vrvaozve.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hwsiwnsq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2yczqkfip.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iompsios.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vdufjugi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bauizpqx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ltlkzsiv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2lvuziifd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xkwrsvap.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rbclkwlt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mxfgwuax.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lvisxqzt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jugkugob.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2adnknivm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ndtjztec.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kymojllm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2yqkwhjrh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zkgvvbmf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qtxzglei.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ivgphwtt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbszerzh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2drdswrmf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tammznks.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2evzenvug.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2awexoirx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oojzssqe.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2injggjcd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2iabpupkv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zxxzrqfb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2aybiqnkz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2biizupbn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tvslkico.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2mrzysqwm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qmwxbzdz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dwhntvme.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hgkmpawx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2plbcoksu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2uuwhvmpq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gyxsxwid.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2emwziixn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2rtqhidum.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yyouodjo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lwzupdye.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2hudwcdsy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2odtyxjyf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2uhgyjzlz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hjmgqbou.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2tqzphbcu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kjzbhmgr.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hjtqwjfu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2rwbxbehj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2xqsadeox.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uarkwiwj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nkvkkjut.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2gcigwavy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rjenogyf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fjirbsxf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2acnplzqd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hwkiylch.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2hecfvvdp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2norrygzp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dntnersh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nngiwghq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2auicrvis.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ksjlbabg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cdelfzwk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fycwjakr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2chjvvwaf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2lvsjsnou.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrmgcqa.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2tkipovnf.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2juttmpyp.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2sajvuubo.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2cumzicka.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2jmzynrqm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2moxurjgp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2qwoqltui.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uhobhwpr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2qdtjpdoy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tfsvkanq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdjlmegk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fzppzpqm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmjzyrw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2olgcttjq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ixgznwlu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2aubfxzpb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vdjvaxpv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2eqhytvwe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgfiwky.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ujpixmod.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zccbdkje.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lxgdjklh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ppruoqrh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wkqujxmb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2pmmqaxai.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2genmbdgr.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2soymtxqp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2itjphfkg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2qgssjugw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rtuqxzlx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hkndyjlw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2rfbcghkd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2amntlslp.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghdtlncz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cydnxkzo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2riryvefp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nihneapg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wsnaejax.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2itnpjfdw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2trvcynyv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kvfhbcee.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhxmzdzc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bnzknxsm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2qaqjxbrt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nezadbtq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vvdndcmj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qkexqusy.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ujyhxipd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpegizd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2wrqqhdfh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hatfpcys.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tujwwptj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2dgijyhbh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cbasmzla.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uptfxghp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyoragii.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2huhxnrbb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tbyupkrg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mmkoayun.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jqhxuwen.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xjrbupzl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xxlgcvyu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2maoykock.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fdqduona.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2njwcmdac.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2zrqpddsd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2kadjzfol.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xffogooi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iyawvgdo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2cjlpamph.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvmbzlri.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hdvuhapt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zwfkyuhb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwqtqgo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmsmvvyj.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vyivvfms.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qsabihda.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2znhnxoqy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sabqcxky.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2sedjrmrj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zknakpaz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2osgsqrkd.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vptgorrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqibgjro.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2hrpkplys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xfjwrahq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lwnjnvok.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2twgeabee.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2pupjecij.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vbljffts.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ubvzsdvi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2retpjlvw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lsuoyota.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ctnsoihm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hgiopbhv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wuwjhutt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2krluikbn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mrwspdyn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcldbrjv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfzzlkp.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2czcsywnq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bysxjgkz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kqcoerhh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tehzlctk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hmqjfend.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2vvivsjmy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fzmkpiip.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tfxekquc.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgnqvjs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ymyrqsbx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pycdmzpe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ilvjbzcz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2znwxulsb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2pegmbsvd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dxpnoopi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gdtwlqkm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fsouqqyn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ndfkunpv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qebptter.html


<!-- 参考信息 -->