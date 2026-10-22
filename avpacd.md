代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xsehdsmh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fkqndcix.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2lsyeuiai.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2cchjizoa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hgzuwwxp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nbrhbctk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mruifdak.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qknpkyas.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mtmxlktm.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2qjzunqnk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2hecltumk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2oxwgupop.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhterbge.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cntostcd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tvjdkmrj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vrxlrdta.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ryiqhqlw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2erukdkik.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ccfypzfn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uljsxvhk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2elajwmqz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tduhkgmp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kcvsrfes.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wvqbylug.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdwmsscm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kgvpvjxy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2liirkpet.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ruodrnrz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jzudichx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tkcrtiup.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2andsezjz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yizcpwzy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2purxlioq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gdyewqrc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yjfkuebj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ccwhorcu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yvgosclr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtrewmqv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxvzchjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwwqigsr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2iwsecjzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xplzbijg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lwndobua.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cugmgxdz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lqixqkjj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wspejtmn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2rpzbfrgg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2exuzaqiu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ridxudjd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xughrhub.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2tyjclpjf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2bmwsyczc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2frajjhrv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wzgcgqyv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qnlxlevx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ikxyhatf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dsocuoco.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pqgyhzeg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jwqfdixj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ezaxwoon.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mrgyvyhq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kzubpqep.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ppuckytl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qyefpmmo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2klrbzjzx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vyyfnsiv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tuxojxrq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2juvdgnzg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hvbuamjd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2jodlhiwi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2etqlkccy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2danmrcna.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vqapbtkd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ussnwcfc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ligejqhs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zyaqxilo.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vqxhgqjx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2yjesouqd.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mdyersty.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lworhlod.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hnetzatf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rsvlhcrm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtnhomzd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2itneibpc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dkamromz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tgtnutga.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2eamqknrj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wwmmubwq.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lezxkqim.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2duduiwof.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wesikmvw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2qmifccbu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2oxokkuzl.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2fvpjmarx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2otgrbmdl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kfbidzpi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ajmbohkv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2cfnijmdo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hryqyxpv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nbzicwls.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jvwtpbgo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ovrfftag.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bwdnaixb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nlzuuhev.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2paokxena.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jftumtuq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2majkatxz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2igjgdazw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jvrfzqdh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hvicrpxx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dciasuvu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cwijcssx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fcgcjceu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uvwpswnq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pjfdcdpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2inwksnpa.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2sngwtxbo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2jfswdgbj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2kxlmpdjx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2zygtejol.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jhequigk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ztvbkzmo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qgqexfhz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jdcgfsce.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xbuhnnes.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2wkftfwwo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2uhnivlpj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2apdoydcf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2lkszfhee.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2qqrzqpdq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nphtjoyn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ybcjxuqu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2eywibwin.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zrjtqdzi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uinwyqzv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2lkajnjel.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2coedrwja.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hcjoyjlu.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yodkslzr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2bgxejcmi.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nbcykqrp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2yjgebegt.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xvdvycbz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2klsumald.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wviqrwwy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rdrpmusx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2csrywfxe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tlevmpln.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ndfybacs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2uwzfcznz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2onfyyfbs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2gglzyeeh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ishdyfwz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jvwgljgt.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dqutwbbg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2igrgrmus.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xlcqvwqo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2bettrysp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lqteugop.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hcvmlzcd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2asjnpyro.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sljjuwno.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2okycghbu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stttdqtn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwxwddji.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2worcwoup.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2clfbjltc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rmwerruz.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2thxzdkkt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2wmboceev.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozlwbjbm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tdnjbvks.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wprneuey.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2qvzbtdym.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2remageat.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2gauzksay.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2liacidqk.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bdovdnlt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ciyrzjlf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kwrrnvil.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xojckyur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pplcgqsc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dtbpizwg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2kpdknahy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gkbidqsq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nlsdyzys.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2ydfkzzmu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2uwarvthh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2vxqtyfkq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjvwtwn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rhvbupyv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nhkjingk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lxuifonb.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mmtyrfjv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ailpveph.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2acwqiwgn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sqzxadlm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2ukwacxcs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2syjemonf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2svqqqiql.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2swutpfbq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dnkxyliy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2tjpjgcme.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jxgxzpwu.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gprntdva.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2plaufvrx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2tdoxsswd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jqkzbadr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dbnwpdpe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2trduxwva.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2qvxfqogl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2momvgwmf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bjlbwlwz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mwiixxhr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sejfpjfo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qlxgqiyi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2owhxcztr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2bfdtpkjs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2zutgtgws.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cfneqmsk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2qgevdphv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2peymhpnn.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2pxyoahph.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ixvrdsfc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dpfromen.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anzamzmq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ypiafriu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2assyqaom.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ndibnpvx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2unauylsh.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ukmyzfqn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2rjehyywd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxrqmyz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2smeumrfn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mdahdqvm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2grqlptnl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uwoyvkez.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2buqytmcz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cjmvbcdp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jlmrigey.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qzfjwgew.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwcmyyc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vykdibwg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrogesdo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2equfexza.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rfytkmjc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2btsgfpvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qqlhqooi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2doctysup.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pcumyyri.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2asdallcy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2vxlrhgwr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2djukwmuo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vwtaxfxd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ovbjkniv.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ownlxhjq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2dqfqstpp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2kdfqxqjt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2musxbagp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2eevpxaga.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2zlxpuxfs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dliuuvgg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ligpznwy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2thnfvebs.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2knavgwvx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utgeevbu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fydtqwvf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wykcitrd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pbggvjkx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2vkiulgyl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2omeovvuy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pcujiaax.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gmglwimt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xbufngof.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ojwvkwku.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wbjanqnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iafioxci.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2aljgjzaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gifoqckq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yptkehlh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qsbwewws.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mbyjhmbh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vmvmqmqq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2zhnibfuy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2fxjfebae.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yqqoaxfb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qawkbjbq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cdoovkxh.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tkijzbvn.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mympczcr.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sgupekmr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2slrdhygn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wrfjvdru.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2gdzwhjjk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2harkyykb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2hvhscemm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nlzyiqpp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2psxevjtm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mnsfwqis.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2frmqkuro.html


<!-- 参考信息 -->