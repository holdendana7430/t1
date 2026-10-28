代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtuuistzle.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gthufecawn.html

wc -l a.txt
来源：http://hz.hnxiangtu.top/gtyulpzbqn.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtqngcjrvx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gzhubu.top/gtfladungx.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtpolexoij.html

diff a.txt b.txt
来源：http://hz.hongshengwenyu.top/gtsmxcmlwf.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gtdsrekvuu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtxuffkjhf.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtfcmqenyi.html

scp file user@host:/path/
来源：http://hz.cashguo.top/gtxnzdryak.html

[R57] 远程执行命令
来源：http://hz.xziqi.cn/gtnogcsthr.html

ssh user@host 'uptime'
来源：http://hz.ehwqpu.com/gthnxhonnj.html

[R58] 下载文件
来源：http://hz.yj20258.top/gtdebdypif.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gtvjytcvbk.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtgzfludyz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yvedp.cn/gtxxgfywjm.html

[R60] 只看 HTTP 状态码
来源：http://hz.ppjwa.cn/gtgoxplybs.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.svipenyu.cn/gtyvupfllt.html

[R61] 磁盘占用
来源：http://hz.mhx1999.top/gtmkcfmmuf.html

df -h;  du -sh *
来源：http://hz.zhiwuduotai.top/gtvvzpwtqx.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gthpqkcgny.html

du -ah . | sort -rh | head -10
来源：http://hz.zycfv.cn/gtoyjetyws.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtqvehuhpm.html

free -h;  ps aux | grep nginx
来源：http://hz.ivvv.top/gtnehqovga.html

[R64] 结束进程
来源：http://hz.meibo888.top/gtsqdriaxu.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtsrrbuoji.html

[R65] 查看端口占用
来源：http://hz.gzhubu.top/gtlhskabwp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtqukiryda.html

[R66] 定时任务
来源：http://hz.yueranfly.top/gtufsnzwsh.html

crontab -e;  crontab -l
来源：http://hz.nanxinkj.top/gtbioxoqgw.html

[R67] 生成随机十六进制串
来源：http://hz.316326.xyz/gtkhcxwbot.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gtxdiflbtt.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtdboogzpa.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dashuyun.cn/gtycuwymzc.html

[R69] 生成随机密码
来源：http://hz.jiagoushi.top/gtysatpfvl.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258888.top/gtpcoexula.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtotqwijfa.html

date +%s;  date -d @1700000000
来源：http://hz.ydjk.org.cn/gtufmvdmrh.html

[R71] 日期格式化
来源：http://hz.ydjk.org.cn/gtshmtrqls.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtxphlwlja.html

[R72] 等待端口就绪
来源：http://hz.hammf.cn/gtngakzlyl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtzmwlbgcx.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtwsginqds.html

split -l 1000 big.log part_
来源：http://hz.jinqigfzy.top/gtyemowjgm.html

[R74] 批量重命名
来源：http://hz.c1oappe.top/gtcakdqhvo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.52xcode.cn/gtkllzeqtb.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtqkhcqcnk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtuqthkkdi.html

[R76] 使用临时文件
来源：http://hz.shuidangran.top/gtcqdkbjyo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtjkvqiyxr.html

[R77] 读取用户输入
来源：http://hz.xinyue.icu/gtuhaxhwgw.html

read -rp "请输入: " ans
来源：http://hz.aizwys.cn/gtavhjvmuj.html

[R78] 交互式菜单
来源：http://hz.gotoacloud.top/gtrrwmrocm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yanxiufei.cn/gthdpjfzxk.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtwjdnorwp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.quarkkingdee.top/gtetkrxvbf.html

[R80] 查看脚本执行耗时
来源：http://hz.316326.xyz/gtaxrouhjm.html

time ./run.sh
来源：http://hz.9152youxi.cn/gtjxtegybq.html

================================================================================
来源：http://hz.guannengcc.top/gtatniluah.html

S. C / C++ 专题
来源：http://hz.quarkkingdee.top/gtxglfcwuy.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbflvxwcx.html

[S01] C：Hello World
来源：http://hz.zhiwuduotai.top/gtjxcvhpyc.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtmzxooben.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtrniiqilu.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtsitkffef.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gtyixopxps.html

[S03] C：读入整数
来源：http://hz.chenzaomai.com/gtcovtihcs.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtdplstfhl.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtksuxxvqk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtgnbdbgsr.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gttoyroica.html

strlen(s)
来源：http://hz.ywan-chungtsiang.top/gtynzfqnzh.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gtwdpxrzaj.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtblpvwtsf.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtftaubpgf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gtudnucrgf.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxinkj.top/gtcfxxejhz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hammf.cn/gtfsjkybut.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gtpalitbfr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xingfuxueyuan.xyz/gtqjpiqrfr.html

[S10] C：指针与解引用
来源：http://hz.gotoacloud.top/gtezhpdbzm.html

int *p = &a;  *p = 5;
来源：http://hz.xylfe.cn/gtadwjamkb.html

[S11] C：逐行读文件
来源：http://hz.xuetiantiany.cn/gtviyrggwk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gtmanlonrx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hfpthk.cn/gtlobmyrst.html

fclose(f);
来源：http://hz.jinqigufen.top/gtlbsgykbd.html

[S12] C：写文件
来源：http://hz.yangfankeji.com/gtvijctfcj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtjtdbyhlj.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtrhfqjmwx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.mhx1999.top/gtttnsxnrb.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtonxnmfop.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xinyue.icu/gtdwkvlqoy.html

[S15] C：类型转换
来源：http://hz.birdmap.top/gtiuxexjhe.html

(double) a / b
来源：http://hz.shuidangran.top/gtlsngkuwa.html

[S16] C：位操作置位
来源：http://hz.sxryk.cn/gtuzjoogvb.html

x |= (1 << 3);
来源：http://hz.ehwqpu.com/gtxjqqpzpd.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtzkagxeua.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yj202588.top/gtamyvarrg.html

[S18] C：命令行参数
来源：http://hz.haohaochexian.top/gtegdugbga.html

int main(int argc, char **argv)
来源：http://hz.svipenyu.cn/gtzvifjfrs.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtbxctvsoc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtlkffobds.html

[S20] C：二分查找
来源：http://hz.gaohongyu789.top/gtxdmzvztb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtdttiwtyf.html

[S21] C：字符类别判断
来源：http://hz.jinyuanbaomall.cn/gtbfvcfybt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtrilvymyi.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtchdnpsyx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.bjfxy.top/gtufqrapje.html

[S23] C：随机数
来源：http://hz.shangyingyoupin.top/gtqrwsqili.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yongpay.top/gtuwcdxnjx.html

[S24] C：获取本地时间
来源：http://hz.nanxinkj.top/gterljwbyb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtqeedwgsh.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gtlsdlrdtt.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtqslqhmfd.html

[S26] C：内存清零
来源：http://hz.zhiwuduotai.top/gtmwzcrqdc.html

memset(a, 0, sizeof a);
来源：http://hz.ydzc1.top/gtglaohzdo.html

[S27] C：定义常量
来源：http://hz.nanxuanxn.top/gtqshaukvr.html

const double PI = 3.14159;
来源：http://hz.jlsjyb.cn/gtqniphdfm.html

[S28] C：静态变量
来源：http://hz.pycfn.com/gththoglxi.html

static int counter = 0;
来源：http://hz.andypj.xyz/gtjiqhiibl.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtrvmnwrhw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtnstkupzw.html

[S30] C：头文件保护
来源：http://hz.daxiang520.top/gtbtnudtsi.html

#ifndef X_H
来源：http://hz.xuanzx.com/gtyhktzgds.html

#define X_H
来源：http://hz.xuetiantiany.cn/gtnpbxuefu.html

#endif
来源：http://hz.cashguo.top/gtdqzkvuqy.html

[S31] C++：Hello World
来源：http://hz.haohaochexian.top/gtcgcivvke.html

#include <iostream>
来源：http://hz.jlsjyb.cn/gtvgfvyidt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.jiagoushi.top/gtfihnrnqj.html

[S32] C++：字符串
来源：http://hz.shangyingyoupin.top/gtswegchoj.html

std::string s = "hi";  s += "!";
来源：http://hz.chenjidiqi.icu/gtqlozhdul.html

[S33] C++：vector 增删
来源：http://hz.svipenyu.cn/gtqnulmeza.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sysykeji.top/gtquctlibs.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtyyshljax.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cdnleiting.top/gtunwombzg.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtfrnkjqas.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtqbyuobhs.html

[S36] C++：unordered_map
来源：http://hz.zhixingplan.top/gtrurkkfnp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtwfrlfzbf.html

[S37] C++：set
来源：http://hz.zhongyouzk.top/gtmyhcbvzs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.vqdsnc.cn/gtbclwfees.html

[S38] C++：排序
来源：http://hz.pycfn.com/gtalccsyts.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtzdwzemxx.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtyhmgcgmm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.pengpengdd.cyou/gtecllocts.html

[S40] C++：查找元素
来源：http://hz.pycfn.com/gtkvbljfld.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.birdmap.top/gtshtmjuou.html

[S41] C++：类与构造函数
来源：http://hz.jinyuanbaomall.cn/gtikntdmta.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.shuidangran.top/gtfcvdavzh.html

[S42] C++：继承与虚函数
来源：http://hz.tanke756.top/gtfokhtzeh.html

class B : public Base { public: void f() override {} };
来源：http://hz.zhoulong.xyz/gtymngbllz.html

[S43] C++：智能指针
来源：http://hz.jinqigfzy.top/gtluehtvfi.html

auto p = std::make_unique<int>(5);
来源：http://hz.hammf.cn/gtgjkjmknp.html

[S44] C++：引用传参
来源：http://hz.jiagoushi.top/gtdracjcit.html

void inc(int &x) { ++x; }
来源：http://hz.zhaomingkeji.xyz/gtlnshvtwx.html

[S45] C++：lambda
来源：http://hz.tianlin.xyz/gtltaojlzi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gthenenarm.html

[S46] C++：函数模板
来源：http://hz.zhaomingkeji.xyz/gtswdxshtc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtsgvulsxq.html

[S47] C++：结构化绑定遍历
来源：http://hz.birdmap.top/gtruizjwhd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gtgzsnbyjg.html

[S48] C++：逐行读文件
来源：http://hz.feifeiyinyue.top/gtaiamnlss.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtgjgngoce.html

while (std::getline(in, line)) { }
来源：http://hz.yongpay.top/gtqzpxehco.html

[S49] C++：写文件
来源：http://hz.gotoacloud.top/gtmldrkkut.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gotoacloud.top/gtcaafklkq.html

[S50] C++：格式化数字
来源：http://hz.smart0.xyz/gtpwgpzsdo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xuanzx.com/gtqunodzdk.html

[S51] C++：显式类型转换
来源：http://hz.pengpengdd.cyou/gtzdacjgjz.html

static_cast<double>(a) / b
来源：http://hz.andypj.xyz/gtwepqvigo.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtnuoagexq.html

int size() const noexcept { return n_; }
来源：http://hz.xylfe.cn/gtrobwrpjm.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtjwtzluub.html

std::vector<int> w = std::move(v);
来源：http://hz.daxiang520.top/gtkljzbjmc.html

[S54] C++：异常处理
来源：http://hz.yj20258.top/gtfsuaxzjb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydzc1.top/gtzzmculdc.html

[S55] C++：结构化绑定
来源：http://hz.jinghuilouyu.cn/gtmqeldfju.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtpfnnxbec.html

[S56] C++：optional
来源：http://hz.aibaodan.cn/gtzqvhkqdb.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gteuarznwd.html

[S57] C++：编译期常量
来源：http://hz.nwbrower.top/gtpoowzaot.html

constexpr int N = 10;
来源：http://hz.fzhhl.top/gtzcaoxqsn.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtoxytqqvk.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydzc1.top/gtvsbbvhcb.html

[S59] C++：静态断言
来源：http://hz.pengpengdd.cyou/gtshuyfhjo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.aibaodan.cn/gtxamvluqb.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtaenfskqc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtxjltthqo.html

================================================================================
来源：http://hz.jiagoushi.top/gtvsudnifg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtdzgcazue.html

================================================================================
来源：http://hz.cheryme.top/gtsqwubwsf.html

[T01] Kotlin：Hello World
来源：http://hz.cashguo.top/gtbkhovqbz.html

println("Hello")
来源：http://hz.xuanzx.com/gtorkoueps.html

[T02] Kotlin：变量
来源：http://hz.9152youxi.cn/gtnvbueisk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258888.top/gtzqehyypi.html

[T03] Kotlin：字符串模板
来源：http://hz.cashguo.top/gtwdokovqh.html

"值: $b"
来源：http://hz.havefunace.top/gtvaqnulvd.html

[T04] Kotlin：空安全
来源：http://hz.bjfxy.top/gtcgfkstus.html

val n: String? = null;  n?.length
来源：http://hz.hnxiangtu.top/gtmrdwgith.html

[T05] Kotlin：when 表达式
来源：http://hz.xylfe.cn/gtvcyuqqro.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ydzc1.top/gtczhcxujw.html

[T06] Kotlin：集合映射
来源：http://hz.quarkkingdee.top/gtnmlbhpzg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.vqdsnc.cn/gtoqtghjpp.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtusbrdwqu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenzaomai.com/gtwyfexshl.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gtjkbfovhl.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtczffixzy.html

[T09] Kotlin：扩展函数
来源：http://hz.xuetiantiany.cn/gtaksdmchl.html

fun String.exclaim() = this + "!"
来源：http://hz.zhengqikj.top/gtqdbvsfvo.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtcyuithao.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhijiandao.cn/gtizmjgadd.html

[T11] Kotlin：协程
来源：http://hz.tian-w.cn/gtfxokeanf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtegsicoir.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtntneknnw.html

val (a, b) = Pair(1, 2)
来源：http://hz.gogol.net.cn/gtwhbemwux.html

[T13] Kotlin：只读 Map
来源：http://hz.shuidangran.top/gtqaxdwhpe.html

val m = mapOf("a" to 1)
来源：http://hz.chenzaomai.com/gtdlrrtdpx.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtthhrwrfc.html

for (i in 1..10) println(i)
来源：http://hz.jianghu66.top/gtphlesmwu.html

[T15] Kotlin：接口
来源：http://hz.chenjidiqi.icu/gtacioxfnh.html

interface Shape { fun area(): Double }
来源：http://hz.9152youxi.cn/gtrhqqadaz.html

[T16] Swift：Hello World
来源：http://hz.aibaodan.cn/gtnqdpumsc.html

print("Hello")
来源：http://hz.shuidangran.top/gtajutcpwl.html

[T17] Swift：变量与常量
来源：http://hz.jlsjyb.cn/gtqqkncciz.html

var a = 1;  let b = 2
来源：http://hz.hysaishi.cn/gtmatofeyf.html

[T18] Swift：字符串插值
来源：http://hz.yonumen.top/gtytspradi.html

"值: \(b)"
来源：http://hz.ydjk.org.cn/gtlrhynxzu.html

[T19] Swift：可选绑定
来源：http://hz.shangyingyoupin.top/gtxjnouapb.html

if let n = opt { print(n) }
来源：http://hz.jianghu66.top/gtkssmzkul.html

[T20] Swift：数组操作
来源：http://hz.yongpay.top/gtdfevdfub.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cucudq.cn/gtfzqddshm.html

[T21] Swift：遍历
来源：http://hz.cqqwz.cn/gtkfoduecl.html

for x in a { print(x) }
来源：http://hz.dashuyun.cn/gtvttllrpv.html

[T22] Swift：字典
来源：http://hz.sysykeji.top/gtvepzlthh.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.andypj.xyz/gtpptfdytf.html

[T23] Swift：函数
来源：http://hz.xingfuxueyuan.xyz/gtinrgnfsu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinqigfzy.top/gtbobicjym.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtseqoxdiu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jlsjyb.cn/gtobxazoou.html

[T25] Swift：结构体
来源：http://hz.jinqigfzy.top/gthartuxkt.html

struct P { var x: Int }
来源：http://hz.9152youxi.cn/gtpocapxsh.html

[T26] Swift：类与重写
来源：http://hz.vqdsnc.cn/gtdouegiqw.html

class A: Base { override func f() {} }
来源：http://hz.hfpthk.cn/gtlmsgwyvm.html

[T27] Swift：错误处理
来源：http://hz.gzhubu.top/gtsrfyetpn.html

do { try f() } catch { print(error) }
来源：http://hz.sxryk.cn/gtvgskwowo.html

[T28] Swift：枚举
来源：http://hz.yuanzhike.top/gtnuncdtfq.html

enum Color { case red, green }
来源：http://hz.smart0.xyz/gttxrnawlu.html

[T29] Swift：guard 提前返回
来源：http://hz.yuanzhike.top/gtudjbsjqv.html

guard let x = opt else { return }
来源：http://hz.hongshengwenyu.top/gtcfczpwzn.html

[T30] Swift：协议
来源：http://hz.nwbrower.top/gtahzgpcvl.html

protocol Shape { func area() -> Double }
来源：http://hz.yanxiufei.cn/gtmxzanmor.html

[T31] Lua：Hello World
来源：http://hz.cdnleiting.top/gtcgtknaoj.html

print("Hello")
来源：http://hz.shanyushiyangtech.top/gtosxnyghd.html

[T32] Lua：局部变量
来源：http://hz.ivvv.top/gtcvgmogti.html

local a = 1
来源：http://hz.xingfuxueyuan.xyz/gtqidgansw.html

[T33] Lua：表（数组）
来源：http://hz.hywenlv.cn/gtdbsgpvug.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.sysykeji.top/gtschqnzwi.html

[T34] Lua：遍历表
来源：http://hz.jinqigfzy.top/gtplujojka.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.vqdsnc.cn/gtlhscjfhw.html

[T35] Lua：字典表
来源：http://hz.jlsjyb.cn/gtqzolzptg.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtkzxalvyv.html

[T36] Lua：函数
来源：http://hz.ydzc1.top/gthmgdpjuc.html

function add(a, b) return a + b end
来源：http://hz.xylfe.cn/gtulvaegap.html

[T37] Lua：字符串拼接
来源：http://hz.nanxuanxn.top/gtevbadcbg.html

"a" .. "b"
来源：http://hz.kuanghao11.cn/gtqwccjdby.html

[T38] Lua：条件
来源：http://hz.zhiwuduotai.top/gtxdnjmvjw.html

if x > 0 then print("正") end
来源：http://hz.hysaishi.cn/gtmvmphxgy.html

[T39] Lua：模式匹配
来源：http://hz.pengpengdd.cyou/gtsvbfohsv.html

string.find(s, "%d+")
来源：http://hz.meibo888.top/gtytsolxvx.html

[T40] Lua：元表
来源：http://hz.zhiwuduotai.top/gtzaogytjl.html

setmetatable({}, { __index = base })
来源：http://hz.xziqi.cn/gtvfwebrys.html

[T41] Perl：Hello World
来源：http://hz.cheryme.top/gtthaeasnj.html

print "Hello\n";
来源：http://hz.ppjwa.cn/gtwmynurgn.html

[T42] Perl：变量类型
来源：http://hz.nanxuanxn.top/gtpypbsldz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.xingfuxueyuan.xyz/gtazgljgkt.html

[T43] Perl：字符串插值
来源：http://hz.yonumen.top/gttxrvscom.html

"值: $a"
来源：http://hz.guannengcc.top/gtxzvfhbga.html

[T44] Perl：条件
来源：http://hz.shuidangran.top/gtdkrbvitv.html

if ($a > 0) { print "正"; }
来源：http://hz.yanxiufei.cn/gtaoawgdpo.html

[T45] Perl：数组遍历
来源：http://hz.ywan-chungtsiang.top/gtlnfmuqty.html

for my $x (@arr) { print $x; }
来源：http://hz.ivvv.top/gtdxrkwwok.html

[T46] Perl：哈希操作
来源：http://hz.ybcxt.top/gtkhyodwju.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.bjfxy.top/gtfusflstw.html

[T47] Perl：正则捕获
来源：http://hz.iojbl.cn/gtvccdxyis.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.yongpay.top/gtllblpdxb.html

[T48] Perl：正则替换
来源：http://hz.sufxvd.cn/gtckaqokhz.html

$s =~ s/old/new/g;
来源：http://hz.yanxiufei.cn/gtjgfjlbgu.html

[T49] Perl：函数
来源：http://hz.yanxiufei.cn/gtkhtdndxx.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.hywenlv.cn/gtcgzjdsge.html

[T50] Perl：逐行读文件
来源：http://hz.ydjk.org.cn/gtbgoqjrgo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.yvedp.cn/gtpjowojwf.html

while (my $line = <$fh>) { print $line; }
来源：http://hz.gogol.net.cn/gtzlgfnaup.html

[T51] Scala：Hello World
来源：http://hz.chenjidiqi.icu/gtzwnusvhn.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtynqqkvge.html

[T52] Scala：变量
来源：http://hz.jlsjyb.cn/gttcwqmbrk.html

val a = 1;  var b = 2
来源：http://hz.nanxinkj.top/gtbchoqsmu.html

[T53] Scala：字符串插值
来源：http://hz.zycfv.cn/gthihvhpkq.html

s"值: $b"
来源：http://hz.sweek.top/gtnaioeltd.html

[T54] Scala：集合映射
来源：http://hz.shanyushiyangkeji.top/gtuhwavmbg.html


<!-- 参考信息 -->