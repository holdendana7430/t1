代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tianlin.xyz/gtwwsctrtz.html

[R48] awk 取指定列
来源：http://hz.ivvv.top/gtyfgiqvih.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtuzlphftv.html

[R49] awk 带条件
来源：http://hz.ybcxt.top/gtcbrlbdur.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shangyingyoupin.top/gtbwvencvn.html

[R50] awk 求和
来源：http://hz.tianlin.xyz/gtatonzosr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtdilqadzk.html

[R51] 排序去重取前几
来源：http://hz.havefunace.top/gtqmwpxfxv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ydjk.org.cn/gtfxvyghiq.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtwjzxikcz.html

wc -l a.txt
来源：http://hz.ybcxt.top/gtklzotgfg.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtavtvlfyf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.52xcode.cn/gtkgnpqufr.html

[R54] 比较两个文件
来源：http://hz.bjfxy.top/gtdkwxaajd.html

diff a.txt b.txt
来源：http://hz.fzhhl.top/gtvuuaupis.html

[R55] 压缩与解压
来源：http://hz.gogol.net.cn/gtfgboauab.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtftotcbiz.html

[R56] 远程拷贝
来源：http://hz.zhixingplan.top/gtnlrbtkmd.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtqcmfkidb.html

[R57] 远程执行命令
来源：http://hz.sysykeji.top/gtmyzuybtl.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtuspxtkav.html

[R58] 下载文件
来源：http://hz.yanxiufei.cn/gtdxpfbavx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jyoumei.cn/gtgswjpfmz.html

[R59] 发 POST JSON
来源：http://hz.fengsongda.top/gtjlgntzen.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jyoumei.cn/gttkxqgvrh.html

[R60] 只看 HTTP 状态码
来源：http://hz.aibaodan.cn/gtzzjgguve.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cheryme.top/gtkfghfcws.html

[R61] 磁盘占用
来源：http://hz.52xcode.cn/gtxwrhfggn.html

df -h;  du -sh *
来源：http://hz.chenjidiqi.icu/gtgxsotbof.html

[R62] 找最占空间的文件
来源：http://hz.guowangkeji.top/gtpvpbixqr.html

du -ah . | sort -rh | head -10
来源：http://hz.chenzaomai.com/gtkrkmrmix.html

[R63] 内存与进程
来源：http://hz.smart0.xyz/gtpzwjtefd.html

free -h;  ps aux | grep nginx
来源：http://hz.nanxinkj.top/gtqxntwunk.html

[R64] 结束进程
来源：http://hz.zhiwuduotai.top/gtwxxultrl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtsehdecrl.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtiuyanptn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtvjmfdnpg.html

[R66] 定时任务
来源：http://hz.jinghuilouyu.cn/gtcoanjecb.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtcqjwxvdz.html

[R67] 生成随机十六进制串
来源：http://hz.wangshuangyany.cn/gterjgxgvo.html

openssl rand -hex 16
来源：http://hz.cdnleiting.top/gthgtudasv.html

[R68] 计算文件校验值
来源：http://hz.sweek.top/gttmkhlbxw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtgiktvkmb.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gtbnmtpwfk.html

head -c 16 /dev/urandom | base64
来源：http://hz.xingfuxueyuan.xyz/gtslihkyvj.html

[R70] 时间戳与互转
来源：http://hz.kuanghao11.cn/gtsskcarcp.html

date +%s;  date -d @1700000000
来源：http://hz.chenjidiqi.icu/gtfmmvoaql.html

[R71] 日期格式化
来源：http://hz.cheryme.top/gtjblraiww.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.haohaochexian.top/gtaufuzzbc.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtdisgxycw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.9152youxi.cn/gtghlwhpnn.html

[R73] 分割大日志
来源：http://hz.0kj1m.cn/gtuolgyymj.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gttzdymcib.html

[R74] 批量重命名
来源：http://hz.zhaomingkeji.xyz/gtahegipev.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xingfuxueyuan.xyz/gtengnmtpn.html

[R75] 导出环境变量
来源：http://hz.shzxlz.cn/gtalnbzkjf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cdnleiting.top/gtfyexcsyy.html

[R76] 使用临时文件
来源：http://hz.shanyushiyangkeji.top/gtmtnflmhh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.haohaochexian.top/gteqzywlzt.html

[R77] 读取用户输入
来源：http://hz.dashuyun.cn/gtnbehkyhq.html

read -rp "请输入: " ans
来源：http://hz.xuanzx.com/gtwsjnchzi.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gtigljddyp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.pycfn.com/gtdnsxjvij.html

[R79] 解析命令行选项
来源：http://hz.nwbrower.top/gtoifoiyjr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hfpthk.cn/gtfdjpnchl.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtjuasnvrc.html

time ./run.sh
来源：http://hz.shuidangran.top/gtmwklwmsv.html

================================================================================
来源：http://hz.hysaishi.cn/gtfpmjmhhv.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtqjlenyvs.html

================================================================================
来源：http://hz.smart0.xyz/gtsldxosml.html

[S01] C：Hello World
来源：http://hz.yj20258888.top/gtdxoqfrsq.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtoqwihflb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shzxlz.cn/gtwqqwcckb.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtmgmbwbhg.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gthrbqaagj.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtkqbzrghf.html

int x; scanf("%d", &x);
来源：http://hz.xziqi.cn/gtbitplhhe.html

[S04] C：字符串复制
来源：http://hz.pengpengdd.cyou/gtqvtwrwkv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtjvrwdrfz.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtuvhiyjvd.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gtcwhjqbhm.html

[S06] C：字符串比较
来源：http://hz.jyoumei.cn/gtwavzqjbd.html

strcmp(a, b) == 0
来源：http://hz.jyoumei.cn/gtavdflgln.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtrvcyxbop.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenjidiqi.icu/gthrdvbbhj.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtdphzvggj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinyuanbaomall.cn/gtfjuvspki.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtmgjzqhja.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangshuangyany.cn/gtecoowfcc.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtvdoisrps.html

int *p = &a;  *p = 5;
来源：http://hz.nwbrower.top/gtmbkjcfif.html

[S11] C：逐行读文件
来源：http://hz.xziqi.cn/gtkhaztjaz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gtciuqehlp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinqigfzy.top/gtbjlkiadg.html

fclose(f);
来源：http://hz.yangfankeji.com/gttaoqzfuo.html

[S12] C：写文件
来源：http://hz.316326.xyz/gtannxdyqg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ehwqpu.com/gtepdheluj.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtkoufmewk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj202588.top/gtujjmeitj.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gtddykimha.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtzrobrctr.html

[S15] C：类型转换
来源：http://hz.aizwys.cn/gtjlhprgwf.html

(double) a / b
来源：http://hz.ppjwa.cn/gtltfyfhmk.html

[S16] C：位操作置位
来源：http://hz.gogol.net.cn/gtpdftqlmb.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtkpnwxbpc.html

[S17] C：安全拼接字符串
来源：http://hz.fzhhl.top/gtpiqccola.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.havefunace.top/gtfbusyozl.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtcmpvzdbe.html

int main(int argc, char **argv)
来源：http://hz.hnqzz.top/gtqksxpkjj.html

[S19] C：快速排序
来源：http://hz.cdnleiting.top/gtsmrojwiu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.mhx1999.top/gtelelcxce.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtqnmidysp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtsmztblwm.html

[S21] C：字符类别判断
来源：http://hz.yonumen.top/gtaemngdvm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jlsjyb.cn/gtgfffhxti.html

[S22] C：字符串转数字
来源：http://hz.yvedp.cn/gtimuskzwp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gotoacloud.top/gtlpvnkdtg.html

[S23] C：随机数
来源：http://hz.yj202588.top/gtumtqrluv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhijiandao.cn/gtuyrwefeb.html

[S24] C：获取本地时间
来源：http://hz.yuxming.cn/gtlmfybzsw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangshuangyany.cn/gtfznbymfl.html

[S25] C：内存拷贝
来源：http://hz.birdmap.top/gthtdgafhk.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtpeuwbbge.html

[S26] C：内存清零
来源：http://hz.tianlin.xyz/gtttetjzzn.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtqwtnrwpz.html

[S27] C：定义常量
来源：http://hz.havefunace.top/gthywsoicd.html

const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtgibpkiwd.html

[S28] C：静态变量
来源：http://hz.jlsjyb.cn/gtsoixhcms.html

static int counter = 0;
来源：http://hz.hywenlv.cn/gtguvfwsiw.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtdujhmccm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.redwolf501.top/gtmuwinhdm.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gtxwfcrsnp.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtbgwjqfwd.html

#define X_H
来源：http://hz.zhengqikj.top/gtcrsfbjrl.html

#endif
来源：http://hz.shangyingyoupin.top/gtghqvhzvg.html

[S31] C++：Hello World
来源：http://hz.zhaomingkeji.xyz/gttwdvleyu.html

#include <iostream>
来源：http://hz.shuidangran.top/gtlknlcfrj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ybcxt.top/gtlodpzbru.html

[S32] C++：字符串
来源：http://hz.nanxinkj.top/gttntetvqd.html

std::string s = "hi";  s += "!";
来源：http://hz.cucudq.cn/gthvptpfdc.html

[S33] C++：vector 增删
来源：http://hz.daxiang520.top/gtsbgifyfo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.9152youxi.cn/gtxpylsytx.html

[S34] C++：遍历 vector
来源：http://hz.xingfuxueyuan.xyz/gtcexzswau.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xuanzx.com/gtkpuecytv.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gteaqdehpl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zycfv.cn/gtdxzrgxld.html

[S36] C++：unordered_map
来源：http://hz.zhongyouzk.top/gtrppdhwej.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangdashe.top/gtwbtqmyco.html

[S37] C++：set
来源：http://hz.guannengcc.top/gtujhfbabl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pycfn.com/gtoskhzumy.html

[S38] C++：排序
来源：http://hz.vqdsnc.cn/gtngtxrqbn.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtcvovzhmu.html

[S39] C++：自定义比较器排序
来源：http://hz.pengpengdd.cyou/gtgdoahuwz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cqqwz.cn/gtxechmuzu.html

[S40] C++：查找元素
来源：http://hz.fengsongda.top/gtdhmuhaln.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.cashguo.top/gtocprtmlv.html

[S41] C++：类与构造函数
来源：http://hz.hnxiangtu.top/gtpxjwdznv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gtgphezjjd.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gttlxhkddd.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258888.top/gtegxhaahn.html

[S43] C++：智能指针
来源：http://hz.guowangkeji.top/gtymwztedk.html

auto p = std::make_unique<int>(5);
来源：http://hz.tanke756.top/gtjwjggnkz.html

[S44] C++：引用传参
来源：http://hz.chenjidiqi.icu/gtnruaqynn.html

void inc(int &x) { ++x; }
来源：http://hz.jinqigfzy.top/gtqzhwncvb.html

[S45] C++：lambda
来源：http://hz.chenjidiqi.icu/gtgexwlqbw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ppjwa.cn/gthvdpckdf.html

[S46] C++：函数模板
来源：http://hz.haohaochexian.top/gtwbjrevjg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tianlin.xyz/gtdtrfjxls.html

[S47] C++：结构化绑定遍历
来源：http://hz.cashguo.top/gtnnvngonf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenjidiqi.icu/gtwcfercva.html

[S48] C++：逐行读文件
来源：http://hz.fzhhl.top/gtcucmojne.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yueranfly.top/gtcruwgcme.html

while (std::getline(in, line)) { }
来源：http://hz.dianchejie.cn/gtrsfosedp.html

[S49] C++：写文件
来源：http://hz.yj20258888.top/gtirpjzslk.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.nanxinkj.top/gtsfiziehi.html

[S50] C++：格式化数字
来源：http://hz.yj20258888.top/gtgavqjmdg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.havefunace.top/gtcurkdbtp.html

[S51] C++：显式类型转换
来源：http://hz.zhoulong.xyz/gtsdoamdtd.html

static_cast<double>(a) / b
来源：http://hz.shangyingyoupin.top/gtbdmjshdn.html

[S52] C++：const 与 noexcept
来源：http://hz.cqqwz.cn/gtoulyihxt.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigufen.top/gtwutybzud.html

[S53] C++：移动语义
来源：http://hz.jianghu66.top/gtchankgmr.html

std::vector<int> w = std::move(v);
来源：http://hz.gotoacloud.top/gtbistkfwy.html

[S54] C++：异常处理
来源：http://hz.jinqigfzy.top/gtjtnkpnja.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yangfankeji.com/gtkavfvwhv.html

[S55] C++：结构化绑定
来源：http://hz.sweek.top/gtzxitkfox.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.haohaochexian.top/gtzfykxllu.html

[S56] C++：optional
来源：http://hz.chenlongwang.top/gthheenmvt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jlsjyb.cn/gtxqtjfvsj.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtilppmjjl.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtdmssfnah.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtezkysfrb.html

namespace ns { int f() { return 1; } }
来源：http://hz.xinyue.icu/gtjabjjmdl.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gthgdotxby.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hywenlv.cn/gtfkwzealr.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gteerioyua.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ybcxt.top/gtbohawhig.html

================================================================================
来源：http://hz.daria6918.cn/gtvbalusqo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.yj202588.top/gtsnfjmowz.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtktctkdhg.html

[T01] Kotlin：Hello World
来源：http://hz.nwbrower.top/gtavblblij.html

println("Hello")
来源：http://hz.yongpay.top/gtfqgmtonj.html

[T02] Kotlin：变量
来源：http://hz.dianchejie.cn/gtoztyymhi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinghuilouyu.cn/gtmyeupbpz.html

[T03] Kotlin：字符串模板
来源：http://hz.sweek.top/gtzfiolcqt.html

"值: $b"
来源：http://hz.smart0.xyz/gtpejtjtfc.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtxqiasnci.html

val n: String? = null;  n?.length
来源：http://hz.zhixingplan.top/gtzfiziqeh.html

[T05] Kotlin：when 表达式
来源：http://hz.aibaodan.cn/gtovmygeah.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.fzhhl.top/gtrmgnerwj.html

[T06] Kotlin：集合映射
来源：http://hz.feifeiyinyue.top/gtbguayqtf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinyuanbaomall.cn/gtwyxdcypi.html

[T07] Kotlin：集合过滤
来源：http://hz.jqgufenzy.top/gtlqnckkux.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.hnqzz.top/gtedligzus.html

[T08] Kotlin：数据类
来源：http://hz.andypj.xyz/gtyyontxum.html

data class User(val name: String, val age: Int)
来源：http://hz.yvedp.cn/gtzorbfijk.html

[T09] Kotlin：扩展函数
来源：http://hz.jianghu66.top/gtjabukhmv.html

fun String.exclaim() = this + "!"
来源：http://hz.xylfe.cn/gtgabnogin.html

[T10] Kotlin：默认参数
来源：http://hz.xingfuxueyuan.xyz/gtmmhccffp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.c1oappe.top/gtrinscedi.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gtbhhqzuwe.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ydzc1.top/gtkldtowdl.html

[T12] Kotlin：解构声明
来源：http://hz.wangdashe.top/gtnxhjvjuv.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtyhhlnlwv.html

[T13] Kotlin：只读 Map
来源：http://hz.yongpay.top/gtskyroalf.html

val m = mapOf("a" to 1)
来源：http://hz.jiagoushi.top/gtxeusrhbe.html

[T14] Kotlin：循环
来源：http://hz.wangshuangyany.cn/gtzwwxdoor.html

for (i in 1..10) println(i)
来源：http://hz.nanxinkj.top/gtqmvcqnlm.html

[T15] Kotlin：接口
来源：http://hz.shangyingyoupin.top/gtxzcnjrok.html

interface Shape { fun area(): Double }
来源：http://hz.zycfv.cn/gtympeyvyk.html

[T16] Swift：Hello World
来源：http://hz.yj20258888.top/gthujnxmmo.html

print("Hello")
来源：http://hz.tanke756.top/gtthmvfqfa.html

[T17] Swift：变量与常量
来源：http://hz.jinqigfzy.top/gtlwsxnspg.html

var a = 1;  let b = 2
来源：http://hz.fengsongda.top/gtmutjpzcs.html

[T18] Swift：字符串插值
来源：http://hz.gogol.net.cn/gtfawmzvhd.html

"值: \(b)"
来源：http://hz.aizwys.cn/gtywmuoorz.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtpqtbvpix.html

if let n = opt { print(n) }
来源：http://hz.gzhubu.top/gtvozuhbkl.html

[T20] Swift：数组操作
来源：http://hz.zhiwuduotai.top/gtctbpvojk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ybcxt.top/gtshucedce.html

[T21] Swift：遍历
来源：http://hz.chenzaomai.com/gthpouryxl.html

for x in a { print(x) }
来源：http://hz.shanyushiyangtech.top/gtrnlkhpzl.html

[T22] Swift：字典
来源：http://hz.xingfuxueyuan.xyz/gttveppofn.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhaomingkeji.xyz/gtmzkjvunz.html

[T23] Swift：函数
来源：http://hz.tanke756.top/gtgjgqvrfv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daxiang520.top/gtibuxseeo.html

[T24] Swift：闭包
来源：http://hz.wangdashe.top/gtrrptqqsq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhoulong.xyz/gtjxcmgogt.html

[T25] Swift：结构体
来源：http://hz.xziqi.cn/gtoizhxxwv.html

struct P { var x: Int }
来源：http://hz.yj202588.top/gtikfbggna.html

[T26] Swift：类与重写
来源：http://hz.gotoacloud.top/gtfisoxsfe.html

class A: Base { override func f() {} }
来源：http://hz.kuanghao11.cn/gtdaqhdpgo.html

[T27] Swift：错误处理
来源：http://hz.guowangkeji.top/gtquguaihy.html

do { try f() } catch { print(error) }
来源：http://hz.yueranfly.top/gtbwcfyiid.html

[T28] Swift：枚举
来源：http://hz.chenzaomai.com/gtamxuqejz.html

enum Color { case red, green }
来源：http://hz.birdmap.top/gtomvlwnoi.html

[T29] Swift：guard 提前返回
来源：http://hz.jinqigfzy.top/gtmbunkspe.html

guard let x = opt else { return }
来源：http://hz.yanxiufei.cn/gtgirprfml.html

[T30] Swift：协议
来源：http://hz.9152youxi.cn/gteugfbjxx.html

protocol Shape { func area() -> Double }
来源：http://hz.andypj.xyz/gtawvupnln.html

[T31] Lua：Hello World
来源：http://hz.birdmap.top/gtemkyskqp.html

print("Hello")
来源：http://hz.gaohongyu789.top/gtkgyxjvry.html

[T32] Lua：局部变量
来源：http://hz.fzhhl.top/gtnmjttgji.html

local a = 1
来源：http://hz.nanxinkj.top/gtmnihkykp.html

[T33] Lua：表（数组）
来源：http://hz.aibaodan.cn/gtazxnapet.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.jqgufenzy.top/gttawlzpai.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtclsvkmam.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.daria6918.cn/gtzimzdzlk.html

[T35] Lua：字典表
来源：http://hz.shanyushiyangkeji.top/gtwjtkhozx.html

local d = { a = 1 };  d.b = 2
来源：http://hz.smart0.xyz/gtdwnymutr.html

[T36] Lua：函数
来源：http://hz.redwolf501.top/gtrlubjzbk.html

function add(a, b) return a + b end
来源：http://hz.52xcode.cn/gtnpyszzda.html

[T37] Lua：字符串拼接
来源：http://hz.ywan-chungtsiang.top/gtkxjciunz.html

"a" .. "b"
来源：http://hz.cdnleiting.top/gtvenyfixv.html

[T38] Lua：条件
来源：http://hz.chenlongwang.top/gtyevmuzja.html

if x > 0 then print("正") end
来源：http://hz.hnqzz.top/gtdvylspmb.html

[T39] Lua：模式匹配
来源：http://hz.0kj1m.cn/gtnadzftqe.html

string.find(s, "%d+")
来源：http://hz.xinyue.icu/gtidnmwllw.html

[T40] Lua：元表
来源：http://hz.nanxinkj.top/gtdpelxogf.html

setmetatable({}, { __index = base })
来源：http://hz.c1oappe.top/gtwosgunwd.html

[T41] Perl：Hello World
来源：http://hz.xingfuxueyuan.xyz/gtkqlnapsf.html

print "Hello\n";
来源：http://hz.xinyue.icu/gtujetnzav.html

[T42] Perl：变量类型
来源：http://hz.daria6918.cn/gthxajacrz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.zdqjudy.top/gtdnlzlyjn.html

[T43] Perl：字符串插值
来源：http://hz.yanxiufei.cn/gtwmsxxied.html

"值: $a"
来源：http://hz.nwbrower.top/gtmwppnmns.html

[T44] Perl：条件
来源：http://hz.jinyuanbaomall.cn/gtigxecscc.html

if ($a > 0) { print "正"; }
来源：http://hz.daria6918.cn/gtvokahspm.html

[T45] Perl：数组遍历
来源：http://hz.birdmap.top/gtafltxlpa.html

for my $x (@arr) { print $x; }
来源：http://hz.jinqigfzy.top/gtlefutmid.html

[T46] Perl：哈希操作
来源：http://hz.ydjk.org.cn/gtrtffplzg.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hz.sysykeji.top/gtfqnhosyy.html

[T47] Perl：正则捕获
来源：http://hz.kuanghao11.cn/gtfvbsbazo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://hz.xingfuxueyuan.xyz/gtmidwunda.html

[T48] Perl：正则替换
来源：http://hz.wangshuangyany.cn/gtzltzoqee.html

$s =~ s/old/new/g;
来源：http://hz.cqqwz.cn/gtvhlpfrvk.html

[T49] Perl：函数
来源：http://hz.nanxuanxn.top/gtqtiqtrua.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.shzxlz.cn/gtdyrqkmod.html

[T50] Perl：逐行读文件
来源：http://hz.316326.xyz/gtdyumcafa.html

open my $fh, "<", "a.txt" or die $!;
来源：http://hz.c1oappe.top/gtbqtqekgc.html


<!-- 参考信息 -->