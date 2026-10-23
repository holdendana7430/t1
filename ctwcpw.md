代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fobudlzr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bmxhkecj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3siukzrsi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lqcouzqd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbkfjxvt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ghoknmha.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wqzwakao.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ihlygikw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qunazyte.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzxoinmz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wnibctrd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rlofrjal.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3waqokhvv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iulmwhug.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3fcvyvngq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hcbvvgko.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsugnvks.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3rtukqyho.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vxegaoyy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qwiicgah.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xsadaqxo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nkoiearp.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wgzghrsc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kuroixyc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ijijsbio.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3akdhgmue.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lktqspby.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uwcenevm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3mhkmmdwp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dqdgdkyq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdzmlgnz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzreqbcw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3osfiwbcr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alesihfg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vybgajuf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vjckcjlv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kromccol.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ekmgomvd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3husfqztf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3znmngors.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vhsuoaly.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pxitfkvn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gitauxki.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zylezyem.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3hjoqtqfz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tpojpvpr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mzgbpubc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uofawcrm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xbuhpogj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3iqadxlzp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3tnjfgnbo.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3kmpqxmtq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ibadlyzn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjbrmgx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ganatoav.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yukycpch.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wojjlisi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wmndovqm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gumhvpbr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3gwauuqig.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sdrkoyhq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3cokfdwam.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wlvbypns.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lmqbxpuk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3hfqhrahw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3fsoozexo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3vtmbvswq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3eijmrztn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xbezawiz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3mcteunba.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iajbwnmy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yqdegscd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nfbumvzy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3upahzfvo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lfgmuljt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cpzdwbva.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ymeyrrtc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zdtayisb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tfnyftro.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uopteqer.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkmqvggq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3borjdkfi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dkhsxxnt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3cktqluzg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ltgbdulo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ljpiyfsy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3lxajrmdi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3obqnljla.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3csbubqik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ydyrgzed.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmsnxtw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kdatxlwq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rrttayrd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hhyfwvjc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3epqzlmsa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3herceilg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ymjhozty.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ejgvjqyl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hbustreu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ityrsepe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3wnlfgdry.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3cdhcbnlx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3raiheuzi.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3remmwxpf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3yktxexal.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lnkxpsdn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hiixijkh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jemnxihy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3boqixayp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3avapibqv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qfhsrpuz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tymqavty.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ywqckvvb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ciovdpoa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eznxjmkt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fmfksziq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dfznlrhw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zhcfmfoq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bzomivkb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nxdhvihz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xendplpa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3sccvptll.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hysxgpjo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3aqtyxjnf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3pbkoizye.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fjtypezy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3dzsxexgr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jlhpisbn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fowndoet.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3qkryqqie.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fitruygv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ndquvfkh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xempiihx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rorkmyid.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3artoeqpx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nihlnkha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zmsfueky.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3utjzmmwu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3slliimgj.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3grwncbnj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3khiddjkr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3kxbanwsp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3coqewptn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3fsjbmtik.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zoyjabfk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ryhgshaq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aencbeuh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ghkwnwsl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xaqdyzhv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zborwtga.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zmkmucxo.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3pxornbmn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rhntmvdi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3oahcxzyg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vupsftei.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hvfvbdkc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sfvqkelc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pizodnev.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3sjcgvonw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ipcthmva.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3puquzthm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3zydccsjj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lqncntyr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bghwivvs.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dsdxfdwe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yviavzwa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3iinqrjex.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ievmxxxf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3sdkupvkr.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3khzhfnkh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ityqhtry.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kvvvexgi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3foekmowq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ntvgntmo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3vnsooccq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3srqxyech.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3eqrbitvg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gtogzuni.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wegmbwtv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xtuktnzh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rbvwcsfe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kldlaowd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pkpozhls.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3czgbdzma.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxbxobds.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hyfcqstj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3uaafxjvr.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ghpjgdzg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3azbqdfmx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ulwwefvn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjifhcv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ekccrkne.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hiynoacm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hutbxhpa.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qqeskgfu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3chyhonuk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mtvlxeai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3edjxesoh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ujfbhzva.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dhufwkrw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ohdjgyla.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wezkrkin.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3lxycxavy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3vksfftgb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3rvmsflgf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ohpubyod.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3nmdmamxq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rdoxpduw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pqnclsud.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3drkuchbb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3slmiiequ.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xcqibjhl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zssvcknt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rylrccrw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3djcqpflk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ruxzhljv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vmskecwg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tcwuzess.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sogofxfh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xwertzrw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxewghjk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bibmwexh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wbszwpoa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gdikklni.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xlsohbcg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qpvhtiou.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3cyqzhxiw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ucvpfoxy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3czhifthd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ckzqkmun.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3odshuvkn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nrtyppve.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3aqruzsed.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uwwfhkoz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3zflrzopm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rbrbvjrn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqecubkn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sivmnbit.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xhuzyynn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3dcrbwhls.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wleiagzm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ixnsracs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vgazvrkn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ulncxzjj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfvumqu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gxhdtrze.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3glcjhdkj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3htqgqwnw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3mnsajsmv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3rbrjrklx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lvrqllck.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ipfljcaq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xvisspvc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hppyopbr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwtimerl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xxnfomyp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3coytxkuz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wukjvabw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3susqakox.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yvfsffxg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3wjcmefcc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwteuaar.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tpbhpdvk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rmftqcxf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xmzldmzy.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xowtqsxx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vptmozxu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhhuimx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsqvewkl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3fvifrbko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulvhppdb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uhgswldv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3guhmxogs.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eewtoubx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wcmmuzca.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zwynpanq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3apvkmfho.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qcjzbscl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3fppnaozs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtclppmv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbycdkwf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3cfrglfbt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3vooerege.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbbopqdp.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lytgisaa.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzvghvt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pahfowwn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3eocbtlad.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yhqxtvgk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ehuiyuwz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lyzyrtlq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bnaocxry.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wzkyyyyg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ktztdyul.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hputkbiz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ysvhamsh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3njdbjgab.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3godgutxt.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qwtvpxcg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hureufzf.html


<!-- 参考信息 -->