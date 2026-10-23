代发 wailian999

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mftxbaos.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yaknynvj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3clvdzpjc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gjahpeqq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3afqgkwwm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hsahcxnk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3yvrkrdjd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zartvsfk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ksumdqqk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lywxbpas.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3zklfykwt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nnrjrmru.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3kflhzmml.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pqvuoidd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3nrhhmyuq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yvvdatlb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cmnsicqn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gidqhhoj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3isdjqgeb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3vhttdlog.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3bfjoehjz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yqqiceho.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bvqopgpt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3djfflqrh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfrofvq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fhanocpj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptklihss.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfouspmu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3tglmlzmy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gjhjdurj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3aztgsktu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rznnsruf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gvdufmpp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rfljstsm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xnvvtexx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zqwwoopc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3evomfylv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jirnwbno.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3noykjrlw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3faydllkw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3mdtmrvbk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ghmecjpx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iveisrcf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sjfrugks.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wjtysjel.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hdemyvar.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3uczetrbi.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qzgnisnk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3oevaeczi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3frcvtvvy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3hamfwjra.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3crhvmlnj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jjrvxnxs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nkdiedix.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3icnropzb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3bajbanjj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ailbtsjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moqhmjlg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ahecgkip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjywttgf.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3iltwitki.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3thtlmthb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jkltrfuo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nwrtmqdv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ruiyszew.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uirequql.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ynocpizf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ooxfayyr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ekaawqmh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zzxnokue.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dbakvwbb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wxsjlkxy.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xpbzcfeo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3txbwuglz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lzhhnvqw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3umvazmdi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bmweomfh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fszsbtid.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3bkqgoxzt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3esrlinja.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3roirasyd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qvkjztmg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3evtqfaky.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3plinwped.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3awkcdmtp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3wegyjfwr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3zmpfjdgh.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3tznhntcj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3bcygukcc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3koflfjik.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yjeivzrl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rghivmav.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdwluxih.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ukhjkrap.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uqmgeazo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3daykmbwf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3brhqyxpk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxvmoutk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3kogjfvlh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3fllztzkb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofehoein.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3iirtupdf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hbnceqec.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvgryvr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3elmyknun.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3nkhjtsvv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fmcmzgzq.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dusrxybs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kjblducc.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lscigrnz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hpzqrttv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3iuumligz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3txwrhpyy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zpsvllnk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qksgphzu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fxklpuhl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tmtksicr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3epobzmwv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3lpvywjjt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cgzqquir.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mtxzippk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3zsvmwsba.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3obqjdlyb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3lgtdodvk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijezdeln.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dgiexblp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gchhgmlt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3blhoewxj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ieqxzslc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3edmneftn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3zgqbnxgh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gtbuqbvv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fshpbyfd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hwtnhyef.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bfferneq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bthbjkzx.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ckcsvnnw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3juxwfnlk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3abgzwkxo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sjeteans.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mvglpycz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oeojynwa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zygihvji.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmhfpkyr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3yjcuudhf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3epdpzgkq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrbrssuy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3jxrvozif.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3vabsfuwz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vgrosddj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rfehnbom.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3txigxyoz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhichxrn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bzsmtimd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3zcwojuxc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wtgnygfr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bkuueqeq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vvxsdwsu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3baoxdtfe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3jfjccerb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3bmbufodq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3stkawdva.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qkcjaduu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wxcgnjeh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uhwzxljk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3zgxxutog.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fiwswano.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uzqduopo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzbdbljr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ajvnhbwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cayakwgp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fskqowlj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3exorhcpg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3rethfhbn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3fjoerhss.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3sfqnnozo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ohiowpye.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3aqbcjsha.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3mphwdjan.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3jxcmaenw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3unglwekv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3htqpbyyh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3vjhwrpau.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wuenqnte.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3cdokmttd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3bmixdaij.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3prbreoqo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3garfgcdp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3okhmwpoz.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3osodjndg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hjoxnutr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bvpgqrzv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3vjjdlefr.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ahzhjnna.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kogwbuyw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3rugggwkw.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3zsnqdxjd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3zeihsjks.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wblhqipu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3tccqbnkp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3kcrqkscb.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3buyqzezj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnsmiktq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xaygkynv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3actbbqee.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3bpfhoefn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3saeeojrp.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3qfjdnzwt.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3hjlgxgyu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3suureclf.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eekoghga.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3cbjkzapn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3wfjmnvrn.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3imykntsg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3yeoakuiq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3tctmshdn.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qbhblyvw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3ojakdxob.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3myiqbaqr.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3fdxikwlc.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3abqummgp.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3tkzfiqog.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3prodosvo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3dmehqndu.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3ipdcfowr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqqitttd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfsdsggk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhthmglg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3gfwveefw.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3cfgfbvcq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lwzonfsk.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3kgcbkzwd.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3tvjzeuar.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3paorerlc.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3kjuorvhp.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dfmwgtab.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3bzffgzvn.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3rrodpfvh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3omsusoub.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qgkjtias.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3otdqnfck.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3kpkikbva.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ejoghevq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uiyudebu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3boarvfwq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xjkojbbe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eodlfxdt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3bwcbanif.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcqzhau.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xgeixebz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xbrzdhxh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3ulcxbcsk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3gbhaadmv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhyfaea.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hdfrwhrn.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3wxrucxla.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3gxfgdfbl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kxvgatcx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3baltbgub.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gznenyxl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cwotnpcr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3wyrgnbiv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3fxvqnqec.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qlamawqb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3kdkbuibl.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dglbeysn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3bykiidtf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3ezgvcqed.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3trltfock.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3jyqkxsvr.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fbfcpgxy.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pycjwade.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3vhocqzjj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3bwjwciqe.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rotdlrzj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3amrsskfa.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3beglcvpg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vxffdygb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvwetpwg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ootxujuv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3sewafvwr.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ouxxxlsx.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3uktxgzhx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3cqbpyhxz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3lxoguotc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qzxlmqgv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3rgxvurug.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvoavmkv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3mpmmrgij.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hxuveiil.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3spfdfcpf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3juenqbbk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pghfhxco.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3esaqbjse.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3ueyybouj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xpvaehcy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3apjrpnxg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3uxvnommk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3repftjzn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eynaxbii.html


<!-- 参考信息 -->