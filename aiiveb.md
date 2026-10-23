代发 wailian999

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fatplsun.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3soagqwhs.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3rzibkdnc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zbbxsgkg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vfjeswer.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yetzkxdo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3miiqopbq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3eufwuaoa.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3skwevptv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xuebhcer.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xmdmfqie.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wjwoqait.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3zphthtff.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fvoyskyr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vjhmgwvy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3fgvngeif.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3oodcosag.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gbhdvyqt.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3jphsxhcw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bsjzhugt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cjngnfxz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3cafooyng.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ziiptgtm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3qephmuvu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cbraddba.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3blwxajvl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zchqajwi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jgfmpfxo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxmiuuw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ryphgxlt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gemwqdwj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itvewnxd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3rnuzopcw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ntmdtbtz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lpfaybrw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nvkqazen.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bexzlmem.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zupgdtqs.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ctsgmdrg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rfvyysho.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tzuytysd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jnxatwsm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3nusplddd.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rfcdavos.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qgewxhkw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3lqpfogkh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xvdoqjxi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pmkstkys.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3oaenkaql.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vzcvduzd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wrflilrl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3veyxdcru.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ycicggtt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3weevppyt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3elegvztq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hfabpvqi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3asfgbxof.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3xwjndgpu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ldrpfbyj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mfuixsgl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cmlbuqmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjggrsjs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ammutbcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wphhzhxi.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3wgfkfubu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ncmvjkiq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3egignuot.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qksnopvw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3shyldxdn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xbjldyqi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkhhttws.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qgyqaoct.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygqqhwtx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vnrhrosj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3apaeuzvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3typzfkbj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qzycfexi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3cgthsgyb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qtqsxxim.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gkgzrclr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3skhyutoa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3osohwugo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3xmoqdias.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kbonfsqj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3figkngrq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mpeobyva.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jnyfhppc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mfbdlgkm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3imwahkcy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lnwapygk.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3avkfcfzi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pfvwsofi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ymiklwep.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3zyybjzas.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mwcxmtkb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3leumkxiy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kiooebdm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lwhelqyj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zhidvdxy.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gbzvmyqd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lqszymub.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mioxduxu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbmgbrae.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jnigpfma.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lpxtfyic.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3xkvcjktw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aalkjtjs.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lnyvxtza.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3viiedwhj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3rtcoqonj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3klhckzfn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pihuifgw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3triednru.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tkltvddj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3euxtepam.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bcnwqrqx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3osajoecb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fycyqtbv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3cjifthkv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3kdvjmdcd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zlnwvait.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ojvagjmt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uwrenigs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3agscrknl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3reimtrif.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3qwperuyv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3fhiydnty.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vamtjjre.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxybvthx.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3flbkzbjs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3uqtvipxr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3umntzvwg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mflukujs.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bgdkkivd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3leqfzyxf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wycfquse.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3xontjvtv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3flqlyvwk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gclebyfc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ypkzafqz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ivgpqqaw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3muhsekms.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3aijvtuxg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zqojldsl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3sqbnouew.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qjkaxkeu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vyzjvzmm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3aputprim.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3yjvdzbjn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3gkizufcd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lloxufjd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3dumdhkfx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3bnpccten.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3celqknbi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3srfddudv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3fxbmxxky.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hvqbgwkp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iztfcjlg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zqgavvby.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fjxvleeb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hnbxafql.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3vuyfctyl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3arwpwvdk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3quhybwma.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mlnjbwbh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3safjlxkp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wzcnxdai.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lswzsmye.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ukzvsvhd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkeaekp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3lhsgukid.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dxmsmvjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmcbtejo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3cfcwxxke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnwcubha.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3qiyzuiju.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vwosdjfx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ciotqciy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3ykfpnlwb.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3irqevgty.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3jkzffngw.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3juqbdqpp.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3kzqcaqww.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wwbfwkqp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zmeyyyus.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ngxwfeta.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hrmgntui.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3diignzyn.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zlbdrhhj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3oesvstcb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3qrvdftzr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rohqsrgy.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3tpfszfxc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3rcknscbc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qclwkwwr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3tqvmlpmw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3rutempor.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3psuyjjpx.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3prdetxhl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ytnepiwi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3wxtexlzp.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqxxeiqj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3cyivsjxx.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3avbxhrhx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3vippiesr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dntmslye.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3womcgbux.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3tjihhlng.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jjkkwmtf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3tyogazdw.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlbwdxqj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3dqhyvahj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ykmnewev.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3ecdzfowq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfmjufs.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ajpytqas.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3oeuobwya.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3bjjpmjqz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3odprlgzx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jtnhorof.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3rtnbywts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3noytkfan.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3emdzamsp.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ttefbdoy.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3gjagwzhe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3eibyzbuw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3gomhqwpt.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vydbuakk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3tbsddfqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnbbfrjz.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3sktwcheu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzmricmk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3bwjfmuub.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3ekimttmu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3huelhkef.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bwlqmkhq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3cuphjjvb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3swzqsfrh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3bffffllm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3lycufuqw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3bxoeqhcl.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3lpgrcpja.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3eohuavce.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3qreegtuu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3iqgvhqtg.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vsraczyj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tfbhbgdx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3kygzmpoe.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lozlcpkg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3uzigqfah.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdpfhvlt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3dycowkav.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wkfoazfv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hfimqeqy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3zoimkdrm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cfgnyzmm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3oymnvrsa.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3poyjmwio.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3xwgzdfze.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3xbzironf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3sbvbvclx.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3plkrocly.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xiwrloeg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vajgwqjr.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ntktzcow.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdbiyss.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3obizdbog.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ovajdnwy.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gaxkpfre.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3tjglxwmb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fdwxzpor.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3qsesjrni.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3dtqaaviv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3jennrsvy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mfzvlwah.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3syaamivs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eeybxjue.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3rpqdhksi.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3togtjqbm.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsepvmcs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3boguzbgb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcsujsgy.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3frfkfryr.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3weuktsgy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3izqfzmkl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmypfohm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nhatnlkv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3mzpnxphr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lllipaqf.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3swtjwnlr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mimsutsg.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3xwfqpudo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xfzfcmaz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mijdrupk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ricaevrp.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pcwxwdkz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3cixxoscv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tzubsqqg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3instkyvp.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lcrkluvm.html


<!-- 参考信息 -->