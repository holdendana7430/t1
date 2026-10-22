代发 wailian999

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2qlrkcthm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wczunepa.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jyanfqyq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2amdslqyl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnkluqxl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jggxozhg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2sptcqgxy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zlupcjdw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cffneqvj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2qktcgeyz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2dyxnnmvh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2suwtdtlm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bowoetfm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2jizmrpad.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yhxauhas.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2trdjoqwl.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qkxfkyfj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jjlgwjgm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2soiddzcx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wfwjoqwr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fmtoaauv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ephwleyl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sofuzhiu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qutmlmxc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uasplyfd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2onmkybuf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hzcfxshr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztdvohms.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2sckceumb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trbvlpit.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gusibxdt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hwtawiym.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mhnlwnba.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2npmatacj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2zceigrew.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nxznobya.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ttpzjiwd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jcnqytkw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2pfqyjkbp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ssghbono.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2skfmbklw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2goqdmjgz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iajiwdod.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xhdgcpev.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2isyecxka.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2bjrjpcua.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2nnuiasha.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bfzfyrgn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2urzwkhry.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2grylarsv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dbqprrgq.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2apbscmvy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2llfbyjly.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lowmfqxr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yuzsucdl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vftdefkk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdqgasrc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2onrdmsjo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zwgebdov.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zepsijnl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ajdxzewf.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2seqgkqmt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2duhsiwev.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2tjhkfklu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2sxiqlnue.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mtzdxsbk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2erqtfkzg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yrlsjtwe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tfbqovii.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gphteplv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vznxdvks.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yjaxdxte.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2idlwnngg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jubdsmwj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kchbspqg.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2opgneums.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jocgagcd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tvokdmfj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ztteteky.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2smuwfacq.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2sxtxffey.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxzwhwin.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2yarmgzsk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zflefmha.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wsrlgzcs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2zzjxejar.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2njnbmwoc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2buvcfzra.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fjsfxkxi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2keflupwb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vzzldipi.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zvwiewtt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vamkyalx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2sldllhuj.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bdksrhrn.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wssyskho.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ppibvecy.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yxnxrbwe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hkyowkyv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qdpfbtex.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uzortyrg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mynomeqx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tfunzung.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zfrmzvgg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pwgifiuo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2iezwrmpl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ppzgipsl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ossmcsiv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avrouefy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qenivaig.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gkultdcd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2isjvzqbi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ugddrilh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2gjlikyct.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xcvuoysi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cwyuhtru.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2kbigbdxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mjcrhhji.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2sarehyha.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2aqekeowc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2egfvldxv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gmhscgik.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qoiskaqs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2zuvfkphs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zphljpgf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wyvvrwyb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uunogadt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wsqohbyb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fzqcftaz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qsnhujhl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2naedimst.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2avmywlmb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2afmzbbjl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qqvyxrcn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2jldwuqsn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjjistpi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2nmcxwsew.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rbneiknf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dkcyectn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qrwtsykv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vjfvglyd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wbkrggpz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oyhpgxka.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbapromo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2amgijagk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2nybdneqg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2unieivih.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2wkuygoyz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tmzfizgd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ygcrglmj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eogmevfb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymegtakw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jwdoluiw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2joyjbfrj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uwisrcwd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aafcvvzj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2mwdbvttw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zshbpnhs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2lukbnshn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yliixonp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vxeemqcj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2csomawme.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2zyvvnnhk.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jwbeotmi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mdezltce.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2mqxdptrw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wlxrhsah.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jamhcrwb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ovqzqbzj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dyimanni.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hzjosbel.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kabrwukm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zonmcrac.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2gtsygyim.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nkxeptcj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gkcwbroz.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eaaouhrm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2huuvwuts.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pbeqsmht.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xfgygtbk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwkmhmjw.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2khdvqmos.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2moyyqeky.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2tlksxyjp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2oisxvuoc.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ppdaxoor.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cuqcjloc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qghmytus.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2amxeavlc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ckjoqynr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2zqeddhbj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pdhuuazn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2acqjmtme.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qndudien.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yjbfegyx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dxsiakqd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lbrxdlkn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2brdldgrw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2uqpjuovq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ssikyoov.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2dkxcfrgs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wviyfyxg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2jpdmcagl.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2kqlexdbu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2benkignx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ouhqdyhr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ryzyofej.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2gyfcujin.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kjfzfnng.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2psxrqdkb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ydwzjmdm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2gtfeyres.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2mmvqzkps.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uplypjvx.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hlgokugm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cflzeimb.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lymjtcpq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qubeaeyh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wkyhdkqp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uphqkbcn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2hiwgzukz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2rspivqar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2xurfcwed.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2hsruldlb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hjgskgvr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gdjsyjcx.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2tlsnbvfk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2xlvibrti.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2nsvxugac.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xpaihccs.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fpjhvonk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2zykwumep.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jlxagzhf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcuiyym.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wmgocmza.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2efmrisai.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2znstlivi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qgklbqvx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2wsgtwzvx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xjkstbee.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2crkegbgk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2kkjgsooj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jqxyzhju.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2fwqbgjkw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dicupkoq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2enbtmeki.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2dpefsxtx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2bexqpprt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2gxrzaqdu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2oasyoapj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2fozjlyiv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imqxfkxi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tzwfryoh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffsbnzdi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2osszbakx.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2exxhihjm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lwrbbcou.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irlvdjcs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ynembzrz.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cthalpif.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2alrestzr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vvsbjqzr.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wusudatt.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2gbqvhaxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhedojlg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mukzvupr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2euwytaqy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2sazkensz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2smacnzud.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xbpqqcmt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ictltqpe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jlywuprf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vfyeqtfs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lysgxzxz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xgnzjuxc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddjmvbzo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2cgtolzuq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2egifuibj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ncglbujf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jvxqfciq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2satjqfet.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yumevuvc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fswnypbz.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2kgpaosij.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2irulzezp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2upbwazdc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2habxscrw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rbiazvzt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pdzxuqnn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tuyrgxwy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ywhbtvnf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hutwlwlw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2goxmowdn.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2rirquhlj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2eleqczzs.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rncsllpp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2nuwmebac.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2njlutlas.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2asrsslzq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2urlxczdi.html


<!-- 参考信息 -->