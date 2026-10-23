代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mhzdvlgy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3unmbnzmi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3eldlrnba.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3luxyeanx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vvnjgdtc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3aohnjlcg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bdoioscr.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ykxbrowa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mbtnbfwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbuuprnx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3lhovmgev.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xjdnfqke.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqtekiem.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3uxemnpqu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bvyfjncg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3aaupzxee.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wfjtgqcc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sazsgmnm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sfhflsna.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ewwryiaa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibwdsrmw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvgayfyl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3omdmmxbb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nlxauogu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ppcqkuci.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ymwplujf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3qorhuxfu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3yfbxbejt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ujfgquke.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mfppisex.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gbwbixyz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3oyqtmpjv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jqvhovcr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xwvrewpl.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hbuptlhk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uictojxn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3zqwjyivf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nytgfrxv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gjukcibm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uvtozxjp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kdubftlk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3spsbvmzx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ufgrbbtj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3atjsiqrh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zpbjgxng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuvighvs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3keftuaps.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3hlflgwlr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3flfxmxzg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wmoqnslk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3oyjhucsq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ctzgiebl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uoxhjvmi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3aiuzwede.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3zsavlhrl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zostrhqs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3luhxtwci.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3lefitxja.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cmvsnvzr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uvmrwbyd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3aefkzjuh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3afalocak.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3whfuazis.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jpciblzf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3guzyjewk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3kjeattbw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wfktdemj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zayafhje.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jnaiybdp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yftbotdn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3pubzklpj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ylqagdyj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kgktveal.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3spxcdnoh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3begnpmsg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3xglzwofz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kqloqkqn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3cordlmds.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3qtupteva.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3dkdufjoi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3xojzfvmv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bjaorefy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3upqxzowr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3flucbuqr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dmzsmrdb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kkjvebxm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dqqijaus.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3kkvszbow.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jfuyjara.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ndpjzhfp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3inekagsf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ukjbtubh.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3irstkihm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nftibyza.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qwfddyur.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bwycekmh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tcczedmx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uesfaisf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pfdjrskq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wzjwssce.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gyidcdmc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ailaopli.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghqhsyyu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3slkggvuh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3weunfsox.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qrwphvcy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nwccfcur.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gbvlkwer.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jmjodinv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xvjrehvd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nkrbadmf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3egocrlym.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pdeofwrs.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nlbarvyj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xorttdkf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3vpzpawup.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bntihghk.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3klvmvdiu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hwpoydrz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ylnyoqdc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqzzejua.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lrflcgcl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wkmmjclr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3yymgkevo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gnlfxjhi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jkyrykdf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3eqoszdkc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xeovedrv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bqwzpxub.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wterimzu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcmjrbc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hotleppx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3gwdwdlfx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3yasxhjio.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cgbwyjpl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xhpsyflk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dgyktzps.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3cvfstnjk.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3kglmwdzi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3adynopqz.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ogfoheba.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zbzvhxpf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptnpisab.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fpdumzde.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rwlwmhlk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qkcxdwbs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3asytpuap.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3avrksusw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ufxyaxny.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kpwbugmh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xdvsppuu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3csqwydth.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ztdflroq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3znnnjbxf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ztnfocpr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lqghayyn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vpkaknfy.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzasftim.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrjiuau.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zycgktgg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3eevfxlod.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qelupjep.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bgljskhx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zowtrywj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mdqfxcls.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3emxnvhfh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pjbshgrf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tldzwbtv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3otngmeff.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qrmnkhnf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mksmtfmt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jogvkrpi.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qhktyxlv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ziqryrcd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rcqawisb.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dkxgptch.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fylthixn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3wtyghfxy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tjfcalbq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kdvsxyjj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3odyalgfz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3plftetyl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3trzzarrt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kuwgnggu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gsheglgm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kjyvutjw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3beqkujkv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ucpdxysc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gtpgpkoj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fpxlinex.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qynjfeca.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zboinlmp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fyksvvvu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3oibnpijj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pcoyqzbe.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cshydsld.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnixjrha.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wwtjauqi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fkzzorwx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3fglldogf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3iommzmhs.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3aonmavee.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mknmefxt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mirrparj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ntnvirqt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3yppvpyar.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3qbfuqwwh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ctykiegw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xbarturg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ewavrnor.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qkbuawli.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3umevywpg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3anzhnwch.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3hsqzaiop.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3zluybrhz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ocdpmahy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3iynnwssf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jfhekrmt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dofftfdf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3oysftvog.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fvptlkkg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hlpsfctk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3vzsvyhac.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ubfnybdj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3zugdadox.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3bkkegvne.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gbhkyzuw.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xzlfwvvx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3uvzdevup.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gufzvdge.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eayusjtl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3glkrlswn.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pcmccgsg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pcwcjefk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oeoqzhbd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3czmibxpo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3atiwgxvf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3tffnlhkj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3brhsikfy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3wmxkoswv.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3nxfxdwtz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ccjvzqvt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3mgdktdny.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zhtzbdxh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xbarztth.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3whaalgzt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uxphokjh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zwchyijd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lptkhbus.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xjxyeybr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3drtvibqz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3takdjwvl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqqbuga.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3opziihmh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3clxkjqgc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jklmddjl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ndnkumad.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3iudaddmt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3hymndujj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cpfziwen.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yaodiwqm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3drsconjp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ujezbjnb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3qprykhfz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dovujvtt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jchgfhxb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3rcpsqjeh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cpbmhyao.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3suvjsnlh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lgsyfykg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xeiuzzoz.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cvsrvyyx.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3fcgyijxr.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rvqzvzin.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3iourpzxy.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hmodxiwf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bqhwdfwm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rhegadwb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gfqdokou.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3phxtcldr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbkduybo.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3paosgmin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yqokgtjy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3npcbpgio.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3pqkrjwrn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hovelbet.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3mmpbnbxq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lyhsyyhc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wdqkcqyg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tzplkvpc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bmnfrpbg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tnmtdyfc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3gkmanmlg.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3jkfuvtup.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mtwmkzmu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aptppzko.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qtvxyyhq.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xjqfyjig.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3hixdcnfs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fwzbbaox.html


<!-- 参考信息 -->