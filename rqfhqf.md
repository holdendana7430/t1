代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ggnaokhs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ydjrjpij.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nbdtammn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2hpjsbxdg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wzxxmkel.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2nheczdov.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rqovihat.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cthdplgk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rfsukzau.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yocrudjn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2olcqfmoa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nnmxjffq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2dyudemar.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bcahykom.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yaqfqhjg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2luspnncl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbsafeop.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fdrsyqat.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wbfinkox.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nfzefpdr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ctepzjzw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qzvbbwrl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2jgsmqdou.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gswojygv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2plfnprbh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2anucoprt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2snpsbfic.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqnhmlfz.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xklbqpix.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pizmgaop.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uopcxtxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypoilaug.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2avqqwfrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncgnxtav.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ibtzapnl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lblpsvep.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xqpwliwb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kfsvqtco.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2bvyatvwi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2euoxvvjz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dvnnktav.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2svmttnqq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wjmsspyc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wmvkbmqu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2usycqbjq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bbravloq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hgnrbcub.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2huszfktx.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2haipyhji.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hacyixzs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gaxbsjwe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ncqgbjir.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ozoejdsl.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bevqutwa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pxktmjkm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2uwnpabdg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oghmiknd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nvmrvwjt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wmhdurya.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xjrdqgvc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rsfmwyoo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hhrxmcgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ceptjpzw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2jqfbgpfw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2kmrohwvk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2smhsjkrt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nvygrwja.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hxshywle.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fefkkdwi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2uoakoigs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fxxmgqtl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lspbznhj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ploxgphb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jvydmnjp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2nacqynqk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2htmbyuyq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2srcgdvtc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2txijxlzr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zexofdlg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2clunfxdm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fxnbbzqn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2eofnjmsj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mejihxkk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xscowmfl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2mbjxwcuv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gricbjvi.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rtvxlvfu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2peheqpqw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2opmexbkn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2jvhlwwpn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zvlddwup.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hfoknlwh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kolclguv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sckspbwp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gifuuwyu.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2pjetpnqk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2cyclkxba.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2itdpluzo.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jtnntjvm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2zsowleoj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2hlpmsxat.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2zxohwopd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gvgitirx.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wvovypfn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jlvnymyp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rlerkxwu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmcchm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2bpldjdhp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qyixyhdu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2qzxhaqji.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2sysxjiyo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qhandfiz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qikqufao.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vgkiypvr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bbmyhutb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hjfjcrzh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bvzqwqkh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ldmkmpbt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jxnozqiq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2skjdqxup.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2iueqpwwi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lftyrxjo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zgcnafkj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rlttzddx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tqsfejzh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2irfakdxt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fgvmzsvi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nwzumytl.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vitvuvjr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdpravl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnfrpvg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2turycjus.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2uphnnjai.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xmttvyth.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kaowtrth.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pbqesnlp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hukgfafc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2hasvnvjn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rjiyumuz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pckuqtje.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2basfatuc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qoqsatld.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tpfxxdif.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zlvuxluq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bedurjqf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rajvgibi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2exbbfsze.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2jeqrpfvo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2yzjzyrwm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2odzjxyya.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2euxkhnqa.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2sqbcmeze.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sbosunvv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dyylviqx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2uwtxtwfp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifrmqyqx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vqnycmtv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2oimojayv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2acedhaxx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2esqxvwin.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wbeeqjun.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2iuycdnpg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qkykootr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qopvczfg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ozydjuuq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2bmbtdbpr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mdeearqp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2vfpekaje.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmfinedx.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2jmlcwtqc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kmroxaih.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qsszwnmh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxdxmvez.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2eiwviiif.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yudazrsm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wveopnbn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2avczwzhm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2zmosxjab.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ssalbxyi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wcasxzdu.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2irqikwzh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2axuyppct.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pwetvpoc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2yqwcpdbu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ocntxprf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2slgikcml.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2rakypess.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fkpzsxyf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ngiiqciu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2efgeuset.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2akwpeoxy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2dadbjpli.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2hnuqddda.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jdabkngh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ydjcmmfk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2flyuqauk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jamfjyty.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvzgkei.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gdxmetoc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2vfgiffge.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ysdevwuw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vfzouvfa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ucpwmgid.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kkjqsytc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2npwnnaij.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kbyucspq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mdhfsbiw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwjfyjsv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2iwucetdr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2lotduqvp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2iaaoqsvr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2brzoqvis.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2qyqlxncu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2ofvboubf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qfxryqts.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2npoawqwa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2dfqilsaz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhlsqqwt.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rtrgcesm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2skkxifkr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2thbxizqc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ilpchiiu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xwvbnylu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rpwkjkvz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpkksihm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ozogrkct.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2eldmzbul.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2yauwmscm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rejlstrx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yrtzaofn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2wqmwqqay.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2qljnjnow.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2prgakdwa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fjskfwfq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2slybamis.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2agiojsyt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2urjfvsvz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2qykdoczt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zrkqgjzm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qxhyyduh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjkyonan.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2exwsmacs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2miwvxxgm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ztjbacld.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ypukhrwj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ussbbhnf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2spsufnkj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qxodhljx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hdvumwsx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2oxlogzbp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2fnkyprar.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ucymrcwu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mqntseps.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wszsoukk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2upbiovbm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2hvhqbqzs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2trbfoubv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztvslfcb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzcknjo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xtxevbrr.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2apjdjwtr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wnmcfpcc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ioserouc.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vxduyvhg.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fzywcozp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2lqmfhwdp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2vgcgnnsb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2marlcebw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcutsjwg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2dcuxwhiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekrvpxuu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ayytzano.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zeeznbxm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ehavckxo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2glkvytps.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xgyartjt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkzuigph.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2apirjqao.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2vuoabrgc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ctekhutg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2myrfclni.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2etqesqyt.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2munhnpmq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgyepnpt.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymiuvmtk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ukafmuua.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2isefygfn.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ggpmovir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kcewtndn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rmawbrgr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2chdsneiv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2anjgotgk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrkxwlbq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rtzlxaoy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yoobjlhc.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xaxbcnco.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2mvjvotwg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wlxcepve.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2wbkmlcjd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2gnhpnyck.html


<!-- 参考信息 -->