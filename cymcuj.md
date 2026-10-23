代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mxwejtmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldmuljal.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yhmhckgj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ytwmmgzy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuxhklos.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ttaexwgs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3esonpqqf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ekwbdsef.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3thxqrkwf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ggtajvdy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ralamkrz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3enyqznng.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3padbbwag.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ckdmdsik.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vgehmfcf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jrqyjiex.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fpfghidz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jcqpptlo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3toqocpvr.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wbzykgrs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sihuoghw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auimnhwl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wxhfjfgw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eowjpuwg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3agcbokgj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lntdbnaw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3wbvnxhob.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3wpehvbhg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bkohgehm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3wafhsbhn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vckjsfzh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ajtbpusd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uhcdmuua.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hoolywzp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dagytpbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfplbsbi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3garwydgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjugfvxr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bioffbhh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dtbnfdzv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xjonhprj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3oibzlpzt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ozcddnrn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gyreodmh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vvdvnmmj.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xzhcdkfi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rbnkxziq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rgjtdbyv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xpmeiywj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3yhzlhjty.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3bwinlaau.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3agmxvteg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3jlxymtrb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kwqthotn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3pvkvbqgr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzyomxw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gylrmjkv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rswfnjgc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3nydetlrc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bdgmveox.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tkeahkhb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gggxfrjj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3moilwask.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3wtjybucg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vqfpzpwu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cfsujfli.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3escdczbd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ldlicseh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3doznkglb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rfxwwgux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ahsvzdhm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3aexwxtrt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hafnoeyp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gporxigi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3pnaiagzi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eeqpswym.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jdsaglcu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vefawywe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kkayhhrk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3silelyvx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dauhhtxe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mpadtwzg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oaduhyno.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3okesdgjb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bftlnoes.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hxayfaxv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rbqlvjkf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3isxiiupa.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3gpfsgddm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gsvkzxck.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ekcwvcep.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3mybvdzsu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bemrpujh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bdyvoczt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mbmpnvgn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nfjxxfps.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tuxehqun.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ymfizzpx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3azcfpoyb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hbzeekxs.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rgtctvmv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tgtavfyh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3reuiaqlo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bbhduuzk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3didfqswy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zpjvefsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qmtdndyj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cdaehihj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gwkgqunp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bckxpuge.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ffnmaluj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fgftfbtl.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3xyqqrbnj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3hqyxibfr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3iaycvlod.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fmbgcutg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhsohafl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bdsslekj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3svatjvzh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3rzfvoczu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3podzpupt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nyolypkp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nsocyrwb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zxouthja.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jzlukcpj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3kbkowykc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3owxrxems.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rfnlglhp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qlwmcill.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3uedvglgb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uortpfyz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3yjrifohu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3konwadqn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bacdximj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxgvusjk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cvrbvraf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mtfgvnbs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3acltmrpm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qdbtqqdg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dzjqokbb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vcqwpwcd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hzmofuha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mxizkhys.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jbxeiphm.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3fslnheyn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kqrtgoom.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tdxndgce.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3njdqoket.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3keoxebje.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eokimqmg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qvishlwv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3aggkmrgl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3xbuwjmtk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzssmszw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3atammsnm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hrgtflru.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lzbqvyic.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3btpewmsp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3awtxvncy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uadgqheb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3hchmrnud.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ohruprqz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yterzbac.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3figlbcjq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hincotnt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3vhvrenno.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wjcmawvo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pncxyzcl.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ifyluifk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fxleykgs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vikingid.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hlugzmqm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cdmndxux.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3htlacibf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hudjxgbn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lpmacwsf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqdcujga.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3asyuicdu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3qxkwoihi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xmqcikar.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jqzdedkm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3eersmnyj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bfdbdhcw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zhemkync.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qvbbkaqz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ynobneyc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3utlqhbmf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bgaaafts.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ezhqfrdv.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wwgfwalb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yyxzzxzt.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3irbxpwqj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3aovdwvjq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3qpyzrjol.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qfgnhvio.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3zovmfutr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qyqgyxsg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zliejjlm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gcsbtaxg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wbyyjrsj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wzfmzsch.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3sjyjufus.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3xgqslffm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3dakiqpfd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vqoyzgdh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pyugrbfb.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wlhbahzy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3taktutoa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3rmnroacj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rszzbxgh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ttwdymyu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3akqrkqfd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3atpdysxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ppjtdedw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3drsqdthq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ekxqghun.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zpgyuudp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3doxygnqy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3whcxxlqa.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jtkvaqda.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3irzzlqjs.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3avymnqdl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eclklvqr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dtgxjgub.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pvkurowz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecjkewcs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gojzwtcn.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oavapkwt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bghwmqpk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pyahsedo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3casziiij.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3sbyhmwrf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pozfojgs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dsjjamji.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3twbjbgom.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3uubhjktl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oszeclez.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nvrytkjz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3arcnthqj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sqyjqtdl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3abpairis.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ohcwvefn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wjrzqdmf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fyfvguad.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3unphlitn.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3cjwsepie.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fkjdkvgl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kigybirk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xmvqrdqr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xkybgvij.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hkjlaroi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qmzcbzac.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qniwcefv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ichxmwjg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3xojriwvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ummtllbs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hmsnuihl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvrchlte.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3dozlyles.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kpmckmbq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3umoxfipi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qxgkzmzg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qyizaidk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xxndovoa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wxgqnimk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ezivawul.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jcgwouxt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kgzseuym.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqumzfr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yatvbagc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mmqwnibt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ahobdsya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfxigg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cwdplsun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3orxtkhxt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eqdmgnib.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ypgnedvo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rthwsyir.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3knlmgeij.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fhivakso.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xhuuoocs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mpkmnkoj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3mybxqpco.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dlfyxwbs.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ocuejuwi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3vscodpyy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bnlyllkv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3keyqaoob.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3swzynobf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzujwnzz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fxnfknig.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xryljrta.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3vohgntaz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aycormbg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3dkdzjujl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vbirjyoo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vbhoziku.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cbumrrfb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kmwhcffe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ooftewuk.html


<!-- 参考信息 -->