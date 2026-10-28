代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtjcvgsghk.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtnsjkqryj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.fengsongda.top/gtllqihnjv.html

[R61] 磁盘占用
来源：http://hz.yuanzhike.top/gtaxfsjjjw.html

df -h;  du -sh *
来源：http://hz.iojbl.cn/gtoarktrve.html

[R62] 找最占空间的文件
来源：http://hz.nanxuanxn.top/gtlneubfkm.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gteqcdtbks.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtfhokowcx.html

free -h;  ps aux | grep nginx
来源：http://hz.havefunace.top/gtluligfed.html

[R64] 结束进程
来源：http://hz.pycfn.com/gtzsvkoqky.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtrspywesp.html

[R65] 查看端口占用
来源：http://hz.zhaomingkeji.xyz/gtikhorvmn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.snrcjt.cn/gtjtlmcklb.html

[R66] 定时任务
来源：http://hz.cashguo.top/gtvcdhjlav.html

crontab -e;  crontab -l
来源：http://hz.cashguo.top/gtbmyvkslb.html

[R67] 生成随机十六进制串
来源：http://hz.chenjidiqi.icu/gtfzeoxytj.html

openssl rand -hex 16
来源：http://hz.aizwys.cn/gtsrwvihbl.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtyuxezkck.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtpghwviqw.html

[R69] 生成随机密码
来源：http://hz.nanxinkj.top/gtbqxvhrzp.html

head -c 16 /dev/urandom | base64
来源：http://hz.316326.xyz/gtfqczhmna.html

[R70] 时间戳与互转
来源：http://hz.yvedp.cn/gtoraraomk.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtvgpeyvmy.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gtzljlhtqc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xingfuxueyuan.xyz/gthzjheygl.html

[R72] 等待端口就绪
来源：http://hz.vqdsnc.cn/gtxsovmdgm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hfpthk.cn/gtkqywlggm.html

[R73] 分割大日志
来源：http://hz.zhongyouzk.top/gtnotuloiq.html

split -l 1000 big.log part_
来源：http://hz.jianghu66.top/gtyvhyyzzi.html

[R74] 批量重命名
来源：http://hz.guannengcc.top/gtoaviduqb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.dashuyun.cn/gtqmtpoutb.html

[R75] 导出环境变量
来源：http://hz.yueranfly.top/gtlkbcpjgc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ybcxt.top/gtqomhevmi.html

[R76] 使用临时文件
来源：http://hz.gotoacloud.top/gtuvshhgpk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtgrtqfbtf.html

[R77] 读取用户输入
来源：http://hz.9152youxi.cn/gtemqwrnyo.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtanxwblym.html

[R78] 交互式菜单
来源：http://hz.9152youxi.cn/gtlzqltsza.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtjpkbhgkj.html

[R79] 解析命令行选项
来源：http://hz.kuanghao11.cn/gtmciupqso.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtxotykfht.html

[R80] 查看脚本执行耗时
来源：http://hz.jinghuilouyu.cn/gtmhfgpcsw.html

time ./run.sh
来源：http://hz.aizwys.cn/gtzhgverss.html

================================================================================
来源：http://hz.yj20258.top/gtrafvhpzn.html

S. C / C++ 专题
来源：http://hz.jinghuilouyu.cn/gtzhfzpjjo.html

================================================================================
来源：http://hz.fzhhl.top/gtwoyekilv.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtejzvzyoh.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtcdnasosc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ivvv.top/gtdbaqdctt.html

[S02] C：变量与格式化输出
来源：http://hz.jianghu66.top/gtixmfuxnk.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtccuroyga.html

[S03] C：读入整数
来源：http://hz.hammf.cn/gtwvsjpkib.html

int x; scanf("%d", &x);
来源：http://hz.smart0.xyz/gtprbkqkyi.html

[S04] C：字符串复制
来源：http://hz.hammf.cn/gtmektmvnv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenjidiqi.icu/gtezyevquo.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtcdsyyuar.html

strlen(s)
来源：http://hz.birdmap.top/gtxbqkwwnl.html

[S06] C：字符串比较
来源：http://hz.xingfuxueyuan.xyz/gtvijgarms.html

strcmp(a, b) == 0
来源：http://hz.yj202588.top/gtvwudrdtq.html

[S07] C：数组遍历求和
来源：http://hz.shanyushiyangtech.top/gtauhnlwcq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.wangdashe.top/gtiybtfczr.html

[S08] C：动态内存分配与释放
来源：http://hz.zhaomingkeji.xyz/gtvvaloqee.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtdysqkcny.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtdqqwzcej.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nwbrower.top/gtbljawcni.html

[S10] C：指针与解引用
来源：http://hz.cqqwz.cn/gtnpbmohfg.html

int *p = &a;  *p = 5;
来源：http://hz.shangyingyoupin.top/gtqisyzwbn.html

[S11] C：逐行读文件
来源：http://hz.sufxvd.cn/gtznwlmwav.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gtijunrzzt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtfwtjrkdw.html

fclose(f);
来源：http://hz.0kj1m.cn/gthqswxrip.html

[S12] C：写文件
来源：http://hz.ybcxt.top/gtedgksazh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtrgkctuna.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtaigakmzr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shangyingyoupin.top/gtuvvtrzxl.html

[S14] C：枚举
来源：http://hz.pycfn.com/gtkhgnnjad.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydzc1.top/gticqozknm.html

[S15] C：类型转换
来源：http://hz.xingfuxueyuan.xyz/gtvxibvzue.html

(double) a / b
来源：http://hz.jinghuilouyu.cn/gtkdkghucd.html

[S16] C：位操作置位
来源：http://hz.zhijiandao.cn/gtvjxnjfix.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtkgfsnmgy.html

[S17] C：安全拼接字符串
来源：http://hz.zhijiandao.cn/gtgrhpokmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daxiang520.top/gtjqkkxddm.html

[S18] C：命令行参数
来源：http://hz.yj20258888.top/gtazcyethu.html

int main(int argc, char **argv)
来源：http://hz.fzhhl.top/gtgxdphfmn.html

[S19] C：快速排序
来源：http://hz.yj202588.top/gtnipbsmih.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtybclhbia.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtmgxostbm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtwgezlysw.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gtamepryya.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cdnleiting.top/gtykltndpu.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtuomimxxz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hfpthk.cn/gtjsizujey.html

[S23] C：随机数
来源：http://hz.ehwqpu.com/gtwscmnrnr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cashguo.top/gthwoqrila.html

[S24] C：获取本地时间
来源：http://hz.bjfxy.top/gtiuroqzbz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.andypj.xyz/gtzolkbanj.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtoljekmts.html

memcpy(dst, src, n);
来源：http://hz.hnxiangtu.top/gtxndkmfau.html

[S26] C：内存清零
来源：http://hz.mhx1999.top/gtguxdzfcy.html

memset(a, 0, sizeof a);
来源：http://hz.gaohongyu789.top/gtllfbhqgf.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtadfsgsyf.html

const double PI = 3.14159;
来源：http://hz.daxiang520.top/gtppvwckfm.html

[S28] C：静态变量
来源：http://hz.tianlin.xyz/gthjynwhyq.html

static int counter = 0;
来源：http://hz.zhijiandao.cn/gtymlxtobo.html

[S29] C：变参函数
来源：http://hz.feifeiyinyue.top/gtblthvrtq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tianlin.xyz/gtlqnnfymp.html

[S30] C：头文件保护
来源：http://hz.hammf.cn/gtedpgmxzu.html

#ifndef X_H
来源：http://hz.yj202588.top/gtpllguzju.html

#define X_H
来源：http://hz.aizwys.cn/gtsgrqzhsd.html

#endif
来源：http://hz.iojbl.cn/gtyutshziy.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtchjgwgdd.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtucipumpi.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gtiugwwcwu.html

[S32] C++：字符串
来源：http://hz.ivvv.top/gtczydnkzd.html

std::string s = "hi";  s += "!";
来源：http://hz.sxryk.cn/gtxymadjfr.html

[S33] C++：vector 增删
来源：http://hz.ehwqpu.com/gthrlnfzee.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtmzttcjug.html

[S34] C++：遍历 vector
来源：http://hz.smart0.xyz/gtfckssyuv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.havefunace.top/gtdjrwxjdy.html

[S35] C++：map
来源：http://hz.guowangkeji.top/gtoyqjjnda.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtmkhfbzkl.html

[S36] C++：unordered_map
来源：http://hz.dianchejie.cn/gthcfasvea.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xuanzx.com/gtaitzfvym.html

[S37] C++：set
来源：http://hz.jlsjyb.cn/gtjxukthrn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gtgyrarqur.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtudpdycil.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangkeji.top/gtrrajvxxm.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtznwafyxh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtzuipuqoj.html

[S40] C++：查找元素
来源：http://hz.nanxinkj.top/gtnehaafeh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hfpthk.cn/gtbxcenpkg.html

[S41] C++：类与构造函数
来源：http://hz.yueranfly.top/gtgqejtioe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gttbbwfftn.html

[S42] C++：继承与虚函数
来源：http://hz.guowangkeji.top/gtttlajess.html

class B : public Base { public: void f() override {} };
来源：http://hz.haohaochexian.top/gthphexzob.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtxoupqabs.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gtnsolzekf.html

[S44] C++：引用传参
来源：http://hz.snrcjt.cn/gtazehbstd.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gtvohbjbzu.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtlkgncpaq.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.shanyushiyangtech.top/gtzzmeyqak.html

[S46] C++：函数模板
来源：http://hz.shuidangran.top/gtioidfisp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zycfv.cn/gtrhcpekzd.html

[S47] C++：结构化绑定遍历
来源：http://hz.iojbl.cn/gtuswruudi.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj202588.top/gtrsuoqazq.html

[S48] C++：逐行读文件
来源：http://hz.chenjidiqi.icu/gtxyxlvwed.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.sweek.top/gtwlhydftx.html

while (std::getline(in, line)) { }
来源：http://hz.sweek.top/gtjotwtrol.html

[S49] C++：写文件
来源：http://hz.hongshengwenyu.top/gtacohsvcz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sweek.top/gtvbayecvw.html

[S50] C++：格式化数字
来源：http://hz.kuanghao11.cn/gtwwopyisx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.haohaochexian.top/gtpezojysh.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gthjvujlxv.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtjcxrcmxk.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtoyklopup.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtglptsjzi.html

[S53] C++：移动语义
来源：http://hz.hnxiangtu.top/gtcztdynkh.html

std::vector<int> w = std::move(v);
来源：http://hz.yonumen.top/gtlqljvpuk.html

[S54] C++：异常处理
来源：http://hz.yanxiufei.cn/gttadiaaix.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xuetiantiany.cn/gtmtritwoz.html

[S55] C++：结构化绑定
来源：http://hz.ppjwa.cn/gtfvwmfhnx.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gtynqinefv.html

[S56] C++：optional
来源：http://hz.andypj.xyz/gtsbrzehaz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jlsjyb.cn/gtvfuwvqpo.html

[S57] C++：编译期常量
来源：http://hz.ehwqpu.com/gtwwddosxt.html

constexpr int N = 10;
来源：http://hz.iojbl.cn/gtkydbsoxz.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtbamefmrk.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhengqikj.top/gtbttjapjy.html

[S59] C++：静态断言
来源：http://hz.gotoacloud.top/gtgtxvkrpu.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sweek.top/gttldxanfz.html

[S60] C++：遍历并删除元素
来源：http://hz.jinyuanbaomall.cn/gtbgvscvme.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.pycfn.com/gtbaujddbh.html

================================================================================
来源：http://hz.zhongyouzk.top/gtnrpfnkpt.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gttjpswhnd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlismplci.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtwdlpgtls.html

println("Hello")
来源：http://hz.birdmap.top/gtxilloiaw.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtbwjrmvcm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hammf.cn/gtxqahazyl.html

[T03] Kotlin：字符串模板
来源：http://hz.52xcode.cn/gtzzpwtnoz.html

"值: $b"
来源：http://hz.yueranfly.top/gtxgflfafw.html

[T04] Kotlin：空安全
来源：http://hz.sysykeji.top/gtshvpzect.html

val n: String? = null;  n?.length
来源：http://hz.wangshuangyany.cn/gtnbdtoehd.html

[T05] Kotlin：when 表达式
来源：http://hz.ehwqpu.com/gtgzwpajwf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hammf.cn/gtrclmfcwp.html

[T06] Kotlin：集合映射
来源：http://hz.haohaochexian.top/gtwgdiedmu.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj20258888.top/gtelrwhbaq.html

[T07] Kotlin：集合过滤
来源：http://hz.cdnleiting.top/gtzmnslqqf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.quarkkingdee.top/gtcxbzesjf.html

[T08] Kotlin：数据类
来源：http://hz.bjfxy.top/gtoazvhaiq.html

data class User(val name: String, val age: Int)
来源：http://hz.cashguo.top/gtqqhgkozv.html

[T09] Kotlin：扩展函数
来源：http://hz.shuidangran.top/gtyamvkkbr.html

fun String.exclaim() = this + "!"
来源：http://hz.yueranfly.top/gtqtdiutit.html

[T10] Kotlin：默认参数
来源：http://hz.tianlin.xyz/gtbuigqdhc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jiagoushi.top/gtvjnqahxt.html

[T11] Kotlin：协程
来源：http://hz.daxiang520.top/gtjjfxeycc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhixingplan.top/gtczlfxuvz.html

[T12] Kotlin：解构声明
来源：http://hz.cqqwz.cn/gtzdxewqjm.html

val (a, b) = Pair(1, 2)
来源：http://hz.bjfxy.top/gtudcdvgqw.html

[T13] Kotlin：只读 Map
来源：http://hz.shangyingyoupin.top/gtjyblrtzo.html

val m = mapOf("a" to 1)
来源：http://hz.dashuyun.cn/gteszhnlcw.html

[T14] Kotlin：循环
来源：http://hz.guowangkeji.top/gtdzdjaszc.html

for (i in 1..10) println(i)
来源：http://hz.yuanzhike.top/gtsakcdalp.html

[T15] Kotlin：接口
来源：http://hz.cheryme.top/gtrvvsbdty.html

interface Shape { fun area(): Double }
来源：http://hz.zhiwuduotai.top/gtznkhhlnq.html

[T16] Swift：Hello World
来源：http://hz.dianchejie.cn/gtduurtuko.html

print("Hello")
来源：http://hz.sxryk.cn/gtlstubvpq.html

[T17] Swift：变量与常量
来源：http://hz.haohaochexian.top/gtkqdzfstr.html

var a = 1;  let b = 2
来源：http://hz.pycfn.com/gtydadbdxv.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtzgeavnln.html

"值: \(b)"
来源：http://hz.tianlin.xyz/gtmzkqqwxi.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtugfdlnzm.html

if let n = opt { print(n) }
来源：http://hz.tianlin.xyz/gtkrakvwve.html

[T20] Swift：数组操作
来源：http://hz.xingfuxueyuan.xyz/gtdmhptnsw.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gthctyufpy.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtzbrejxsl.html

for x in a { print(x) }
来源：http://hz.jinghuilouyu.cn/gtvjtmtjcq.html

[T22] Swift：字典
来源：http://hz.jinqigufen.top/gttzxyyrjl.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cashguo.top/gtozongwrp.html

[T23] Swift：函数
来源：http://hz.jlsjyb.cn/gtakompuls.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gtapkvrxzb.html

[T24] Swift：闭包
来源：http://hz.fengsongda.top/gtydwhwzto.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhoulong.xyz/gtaubnafxy.html

[T25] Swift：结构体
来源：http://hz.xingfuxueyuan.xyz/gtthdwavjs.html

struct P { var x: Int }
来源：http://hz.yuanzhike.top/gtwzdxqaua.html

[T26] Swift：类与重写
来源：http://hz.sweek.top/gtbjzhreej.html

class A: Base { override func f() {} }
来源：http://hz.pycfn.com/gtuttttlbf.html

[T27] Swift：错误处理
来源：http://hz.sufxvd.cn/gtcfepivws.html

do { try f() } catch { print(error) }
来源：http://hz.hnxiangtu.top/gtizvxefly.html

[T28] Swift：枚举
来源：http://hz.yj20258.top/gtpvyfddly.html

enum Color { case red, green }
来源：http://hz.yangfankeji.com/gtwhkbafhw.html

[T29] Swift：guard 提前返回
来源：http://hz.fengsongda.top/gtzhhctcfd.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtewtxidmr.html

[T30] Swift：协议
来源：http://hz.cheryme.top/gtpaboigqe.html

protocol Shape { func area() -> Double }
来源：http://hz.gotoacloud.top/gtbrmradlf.html

[T31] Lua：Hello World
来源：http://hz.vqdsnc.cn/gtsoupqlzc.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtqqhruqei.html

[T32] Lua：局部变量
来源：http://hz.fzhhl.top/gtamlrkryc.html

local a = 1
来源：http://hz.shangyingyoupin.top/gtoofddivh.html

[T33] Lua：表（数组）
来源：http://hz.pycfn.com/gtrudmdbwr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ydjk.org.cn/gtwuqsnzwd.html

[T34] Lua：遍历表
来源：http://hz.hysaishi.cn/gtyozqppyi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.ybcxt.top/gtearmwhaf.html

[T35] Lua：字典表
来源：http://hz.316326.xyz/gtdoxtizop.html

local d = { a = 1 };  d.b = 2
来源：http://hz.nwbrower.top/gtzijrtlbd.html

[T36] Lua：函数
来源：http://hz.316326.xyz/gttlpijlhi.html

function add(a, b) return a + b end
来源：http://hz.tian-w.cn/gtghjhwubl.html

[T37] Lua：字符串拼接
来源：http://hz.xuetiantiany.cn/gtpvbezfty.html

"a" .. "b"
来源：http://hz.daxiang520.top/gtiiijsyff.html

[T38] Lua：条件
来源：http://hz.mhx1999.top/gtdeyqzeqc.html

if x > 0 then print("正") end
来源：http://hz.zhoulong.xyz/gtrqbmredx.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtkxcumxig.html

string.find(s, "%d+")
来源：http://hz.chenjidiqi.icu/gtwkpqieiu.html

[T40] Lua：元表
来源：http://hz.zdqjudy.top/gtwmcfecjm.html

setmetatable({}, { __index = base })
来源：http://hz.zhengqikj.top/gtqdzoehyc.html

[T41] Perl：Hello World
来源：http://hz.yvedp.cn/gttiqdvyxx.html

print "Hello\n";
来源：http://hz.hongshengwenyu.top/gtkaffpbww.html

[T42] Perl：变量类型
来源：http://hz.wangdashe.top/gtqparnkxe.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.cheryme.top/gtuvricqzf.html

[T43] Perl：字符串插值
来源：http://hz.ybcxt.top/gtgeejqizs.html

"值: $a"
来源：http://hz.zdqjudy.top/gtktksflhy.html

[T44] Perl：条件
来源：http://hz.cucudq.cn/gtjfymanit.html

if ($a > 0) { print "正"; }
来源：http://hz.wangshuangyany.cn/gtsslmxgqt.html

[T45] Perl：数组遍历
来源：http://hz.pycfn.com/gtlpnrvhvu.html

for my $x (@arr) { print $x; }
来源：http://hz.hfpthk.cn/gtoertbwta.html

[T46] Perl：哈希操作
来源：http://hz.sysykeji.top/gthflwqnck.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.kuanghao11.cn/gtkadxnoci.html

[T47] Perl：正则捕获
来源：http://hz.wangshuangyany.cn/gtmpggeprj.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.ywan-chungtsiang.top/gtnmdlwcka.html

[T48] Perl：正则替换
来源：http://hz.svipenyu.cn/gtofhnuosj.html

$s =~ s/old/new/g;
来源：http://hz.ydjk.org.cn/gttdddtxcr.html

[T49] Perl：函数
来源：http://hz.hywenlv.cn/gthvqlyolg.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.mhx1999.top/gtpxarvzer.html

[T50] Perl：逐行读文件
来源：http://hz.jinqigfzy.top/gtyjlcvsfx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.snrcjt.cn/gtzoohvgcf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.cucudq.cn/gtutcpmuih.html

[T51] Scala：Hello World
来源：http://hz.zhiwuduotai.top/gtnclpjryk.html

println("Hello")
来源：http://hz.hongshengwenyu.top/gtcikhzcrk.html

[T52] Scala：变量
来源：http://hz.fengsongda.top/gthizhcbvh.html

val a = 1;  var b = 2
来源：http://hz.yuanzhike.top/gtkmxapcpp.html

[T53] Scala：字符串插值
来源：http://hz.guowangkeji.top/gttxeweoku.html

s"值: $b"
来源：http://hz.yanxiufei.cn/gtnoakytbn.html

[T54] Scala：集合映射
来源：http://hz.gaohongyu789.top/gtffnmezpm.html

List(1, 2, 3).map(_ * 2)
来源：http://hz.gogol.net.cn/gtcmxulhgp.html

[T55] Scala：集合过滤
来源：http://hz.yj20258888.top/gtzzphucia.html

List(1, 2, 3).filter(_ > 1)
来源：http://hz.tianlin.xyz/gtfqplfwbe.html

[T56] Scala：样例类
来源：http://hz.xingfuxueyuan.xyz/gttukxwzqr.html

case class User(name: String, age: Int)
来源：http://hz.yvedp.cn/gthlbpmvkz.html

[T57] Scala：模式匹配
来源：http://hz.shanyushiyangkeji.top/gtqvefpwmu.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://hz.zhaomingkeji.xyz/gttbwbuisq.html

[T58] Scala：函数定义
来源：http://hz.shuidangran.top/gtidhktwkb.html

def add(a: Int, b: Int): Int = a + b
来源：http://hz.snrcjt.cn/gtjiacdawq.html

[T59] Scala：循环
来源：http://hz.jinqigfzy.top/gtgtqggwca.html

for (i <- 1 to 10) println(i)
来源：http://hz.zhiwuduotai.top/gtwwfqdkhr.html

[T60] Scala：折叠
来源：http://hz.hywenlv.cn/gtybziqiyg.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://hz.sweek.top/gtzsnhrwml.html

================================================================================
来源：http://hz.yangfankeji.com/gtpxsfaqdf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hz.pycfn.com/gtpywhjatf.html

================================================================================
来源：http://hz.meibo888.top/gtgaghvrsz.html


<!-- 参考信息 -->