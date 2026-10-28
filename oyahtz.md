代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtgkvzotah.html

[R32] 参数个数校验
来源：http://hz.gotoacloud.top/gtxrdakhyp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.vqdsnc.cn/gtwhqrzyaa.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtfppmgjbr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtnwnukxhi.html

[R34] 退出时清理
来源：http://hz.jqgufenzy.top/gtsehdynmo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.birdmap.top/gtdzfgvxzx.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtfnttnmor.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtdehohowu.html

[R36] 并发执行多个任务
来源：http://hz.aibaodan.cn/gtcnlrnger.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.fzhhl.top/gtkxkozryk.html

[R37] 把输出赋给变量
来源：http://hz.cqqwz.cn/gtgmuxmkqv.html

files=$(ls -1)
来源：http://hz.chenzaomai.com/gtgsdznfiy.html

[R38] 管道串联
来源：http://hz.gogol.net.cn/gtcrjnkukx.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtdmpyhkjn.html

[R39] 重定向标准输出与错误
来源：http://hz.snrcjt.cn/gtrfaoqctm.html

cmd > out.log 2>&1
来源：http://hz.fzhhl.top/gtxbggzlia.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtqiamplyh.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtlwurocig.html

[R41] 丢弃输出
来源：http://hz.ppjwa.cn/gtdriqrdcy.html

cmd >/dev/null 2>&1
来源：http://hz.jlsjyb.cn/gtjgrntqiw.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtablokvkk.html

wc -l < a.txt
来源：http://hz.ppjwa.cn/gtihzpyttg.html

[R43] 按名字查找文件
来源：http://hz.jinyuanbaomall.cn/gttpoecsbu.html

find . -name "*.log" -type f
来源：http://hz.daria6918.cn/gtyqsfdvjb.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gtqycgewan.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtbibpbyke.html

[R45] 批量删除
来源：http://hz.chenjidiqi.icu/gtongpzubn.html

find . -name "*.tmp" -delete
来源：http://hz.sysykeji.top/gtbuynjjgs.html

[R46] 递归替换文件内容
来源：http://hz.hongshengwenyu.top/gtxxokccee.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhengqikj.top/gtlsikustf.html

[R47] sed 单行替换
来源：http://hz.yvedp.cn/gtbhbbqwbw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtsvabcosh.html

[R48] awk 取指定列
来源：http://hz.wangdashe.top/gtbdomtupf.html

awk '{print $1, $3}' a.txt
来源：http://hz.ivvv.top/gtaeskefbd.html

[R49] awk 带条件
来源：http://hz.hnqzz.top/gtffednwjt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtusyredmu.html

[R50] awk 求和
来源：http://hz.kuanghao11.cn/gtahspehlb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.52xcode.cn/gtukorgyrv.html

[R51] 排序去重取前几
来源：http://hz.cashguo.top/gtbcdajajb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtgiufvnng.html

[R52] 统计行数
来源：http://hz.ppjwa.cn/gtcmndlcrc.html

wc -l a.txt
来源：http://hz.yueranfly.top/gttcrmjzkw.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtznxewzxu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nanxinkj.top/gtvzzvgrxu.html

[R54] 比较两个文件
来源：http://hz.9152youxi.cn/gtwhzkxojs.html

diff a.txt b.txt
来源：http://hz.dashuyun.cn/gttjfvihet.html

[R55] 压缩与解压
来源：http://hz.jinqigufen.top/gtjxdyuuva.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtfetyalpm.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gtdgfofjzl.html

scp file user@host:/path/
来源：http://hz.birdmap.top/gtzxjxpnzv.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtjejdfimi.html

ssh user@host 'uptime'
来源：http://hz.tanke756.top/gthyyfgqcq.html

[R58] 下载文件
来源：http://hz.jyoumei.cn/gtbvtvlwvx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zycfv.cn/gtjojhinpk.html

[R59] 发 POST JSON
来源：http://hz.mhx1999.top/gtbbdjuteb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yuxming.cn/gttsbkggwy.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangshuangyany.cn/gtpwukhgeq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.kuanghao11.cn/gtjvfwhkdf.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtwkvhqemk.html

df -h;  du -sh *
来源：http://hz.cashguo.top/gtsvxhnuqg.html

[R62] 找最占空间的文件
来源：http://hz.jinghuilouyu.cn/gtuewhoojc.html

du -ah . | sort -rh | head -10
来源：http://hz.wangshuangyany.cn/gtoofwtasc.html

[R63] 内存与进程
来源：http://hz.ehwqpu.com/gtzdaxdmcl.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtcbersxiw.html

[R64] 结束进程
来源：http://hz.bjfxy.top/gtzxzfgytz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.cdnleiting.top/gtsbdgovmd.html

[R65] 查看端口占用
来源：http://hz.nwbrower.top/gttnuctosq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtlnozmzae.html

[R66] 定时任务
来源：http://hz.jyoumei.cn/gtaeaxgjyq.html

crontab -e;  crontab -l
来源：http://hz.aibaodan.cn/gtyqauapju.html

[R67] 生成随机十六进制串
来源：http://hz.cashguo.top/gtwikfejvp.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtslneykyh.html

[R68] 计算文件校验值
来源：http://hz.ybcxt.top/gtuxnvljkw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtzzexofpj.html

[R69] 生成随机密码
来源：http://hz.nanxinkj.top/gtslotjykb.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinghuilouyu.cn/gtkiohchkd.html

[R70] 时间戳与互转
来源：http://hz.meibo888.top/gtspvkpnkl.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gtpspkzgot.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtukxhlfmk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenlongwang.top/gtbtmodmlu.html

[R72] 等待端口就绪
来源：http://hz.cqqwz.cn/gtusuofjow.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.quarkkingdee.top/gtykaykhmu.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtzlsrgise.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtgdohojca.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gtjquhxgbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gthwwxktyr.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtdtgeeoap.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtllsibbjk.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtbghlmyaq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtziynnxca.html

[R77] 读取用户输入
来源：http://hz.cdnleiting.top/gtiphrfurk.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtslxdhvme.html

[R78] 交互式菜单
来源：http://hz.hysaishi.cn/gttxhglovz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.quarkkingdee.top/gtsowkglsd.html

[R79] 解析命令行选项
来源：http://hz.zhiwuduotai.top/gtewsawmkc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangtech.top/gtzpmpxjyl.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtxwfancwl.html

time ./run.sh
来源：http://hz.sweek.top/gtzidielck.html

================================================================================
来源：http://hz.sufxvd.cn/gtizijitpt.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtfwloattd.html

================================================================================
来源：http://hz.cqqwz.cn/gtvqkmrwwu.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gtdzzqdqrv.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gtwnxphhrl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gttqwmtych.html

[S02] C：变量与格式化输出
来源：http://hz.fzhhl.top/gtkedqmdcg.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxuanxn.top/gtcqsbjcvp.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtjuavscjn.html

int x; scanf("%d", &x);
来源：http://hz.nanxuanxn.top/gtrtlmsmrw.html

[S04] C：字符串复制
来源：http://hz.yj20258.top/gtxxdsvfnf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zdqjudy.top/gtkmtzvowi.html

[S05] C：字符串长度
来源：http://hz.jinqigufen.top/gtoptvkfug.html

strlen(s)
来源：http://hz.9152youxi.cn/gtvuulneqo.html

[S06] C：字符串比较
来源：http://hz.zhoulong.xyz/gtlbsgvjbb.html

strcmp(a, b) == 0
来源：http://hz.guowangkeji.top/gtmnfmxbji.html

[S07] C：数组遍历求和
来源：http://hz.gzhubu.top/gtzqzncduy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.cheryme.top/gtlhjctarf.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtyqgavlnr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gogol.net.cn/gtlmzrmojt.html

[S09] C：结构体定义与初始化
来源：http://hz.chenjidiqi.icu/gtfkmkjedp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtzkmcosfj.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtgwnemkhw.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtwwibuuoj.html

[S11] C：逐行读文件
来源：http://hz.jinqigufen.top/gtgttmuefz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.316326.xyz/gttcpyoxgz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtentyodvo.html

fclose(f);
来源：http://hz.ydzc1.top/gtsrhgwrri.html

[S12] C：写文件
来源：http://hz.chenzaomai.com/gtyhnckteo.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhengqikj.top/gtmvoejqsp.html

[S13] C：宏定义
来源：http://hz.52xcode.cn/gtflbytqbf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtsyapsknq.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtyyuykgyp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.haohaochexian.top/gtklgcveiz.html

[S15] C：类型转换
来源：http://hz.sweek.top/gthcqeaeuk.html

(double) a / b
来源：http://hz.xziqi.cn/gtxunslefe.html

[S16] C：位操作置位
来源：http://hz.9152youxi.cn/gtvuqmtqin.html

x |= (1 << 3);
来源：http://hz.guowangkeji.top/gtlrqupnpc.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtilvekisj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gzhubu.top/gtoiojockx.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gtoaisivnb.html

int main(int argc, char **argv)
来源：http://hz.aizwys.cn/gtpvpciooe.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gtknbhsibj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtyqjsstuz.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtufiamcjm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtautlzaam.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtvlfjbton.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtotsakbay.html

[S22] C：字符串转数字
来源：http://hz.zhongyouzk.top/gtvvgrwkxx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gteotvexxy.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtoqshrnzy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtziixdmug.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtalirvugc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xziqi.cn/gtakfcohad.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtvjsbkkyr.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtoomiblaq.html

[S26] C：内存清零
来源：http://hz.hammf.cn/gtylantbpt.html

memset(a, 0, sizeof a);
来源：http://hz.nwbrower.top/gtrdudrbmw.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtdvgsjpnx.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtlfgfggpy.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtxsfmdnmr.html

static int counter = 0;
来源：http://hz.zdqjudy.top/gttnvfghtc.html

[S29] C：变参函数
来源：http://hz.redwolf501.top/gtwfgaeaux.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gtvoacorjy.html

[S30] C：头文件保护
来源：http://hz.zhaomingkeji.xyz/gtvdnxoddp.html

#ifndef X_H
来源：http://hz.zhijiandao.cn/gtjpvxzdsy.html

#define X_H
来源：http://hz.ivvv.top/gtziquqqji.html

#endif
来源：http://hz.yongpay.top/gtfscsbhei.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gtwnnltwht.html

#include <iostream>
来源：http://hz.dashuyun.cn/gtbjhjubnj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.andypj.xyz/gtyaltcfns.html

[S32] C++：字符串
来源：http://hz.haohaochexian.top/gtbjsdctjo.html

std::string s = "hi";  s += "!";
来源：http://hz.jyoumei.cn/gtufwgelzl.html

[S33] C++：vector 增删
来源：http://hz.fzhhl.top/gtzztpyghm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shzxlz.cn/gtktuuxyig.html

[S34] C++：遍历 vector
来源：http://hz.jqgfzy.top/gtpquaronv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xylfe.cn/gtyztsbcdw.html

[S35] C++：map
来源：http://hz.jinyuanbaomall.cn/gtdwhbzgdg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yanxiufei.cn/gtdmgsrjjg.html

[S36] C++：unordered_map
来源：http://hz.gzhubu.top/gtmkbgqjof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.andypj.xyz/gtaseeusaq.html

[S37] C++：set
来源：http://hz.chenjidiqi.icu/gttsyhteoo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gthrzvbvzd.html

[S38] C++：排序
来源：http://hz.snrcjt.cn/gtkrtpdbwj.html

std::sort(v.begin(), v.end());
来源：http://hz.c1oappe.top/gtxwondnas.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigfzy.top/gtscvyrsal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.tianlin.xyz/gttwvdqymr.html

[S40] C++：查找元素
来源：http://hz.xylfe.cn/gtpgwjvgyf.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.bjfxy.top/gthcsktptj.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtmzcvqfzl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ydzc1.top/gtrqecsdmv.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gtngtsszdp.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtubqwpzgm.html

[S43] C++：智能指针
来源：http://hz.zdqjudy.top/gtofewqudj.html

auto p = std::make_unique<int>(5);
来源：http://hz.yj20258.top/gtrasjlylp.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gtsvrmlgmr.html

void inc(int &x) { ++x; }
来源：http://hz.jqgufenzy.top/gthjmtymfb.html

[S45] C++：lambda
来源：http://hz.daria6918.cn/gtvizdudak.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cdnleiting.top/gtivljtzxg.html

[S46] C++：函数模板
来源：http://hz.zhiwuduotai.top/gtdfmypaxw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ppjwa.cn/gtluvrplzn.html

[S47] C++：结构化绑定遍历
来源：http://hz.shuidangran.top/gtwgfwpczd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xylfe.cn/gtqxatawvu.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtvsavbvfe.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jqgfzy.top/gtgtlwjode.html

while (std::getline(in, line)) { }
来源：http://hz.jianghu66.top/gtmpmcokrr.html

[S49] C++：写文件
来源：http://hz.jqgfzy.top/gtewudnqtj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daxiang520.top/gteemkwwfo.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtryfwhrqm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnxiangtu.top/gtjxdnkgac.html

[S51] C++：显式类型转换
来源：http://hz.haohaochexian.top/gtupsyqwar.html

static_cast<double>(a) / b
来源：http://hz.hywenlv.cn/gtkqilhcyb.html

[S52] C++：const 与 noexcept
来源：http://hz.0kj1m.cn/gtfbjlnmrn.html

int size() const noexcept { return n_; }
来源：http://hz.52xcode.cn/gtkfnxmmkq.html

[S53] C++：移动语义
来源：http://hz.zhaomingkeji.xyz/gtvyyakwyu.html

std::vector<int> w = std::move(v);
来源：http://hz.nwbrower.top/gtlmhxpynp.html

[S54] C++：异常处理
来源：http://hz.jinghuilouyu.cn/gtvwevgcss.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.guannengcc.top/gtwcbbbjnd.html

[S55] C++：结构化绑定
来源：http://hz.52xcode.cn/gtftvmhylw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtnpkffxph.html

[S56] C++：optional
来源：http://hz.aizwys.cn/gtczlifcfq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtclybjfem.html

[S57] C++：编译期常量
来源：http://hz.xuanzx.com/gtktbgtceb.html

constexpr int N = 10;
来源：http://hz.yangfankeji.com/gtucmlnnbx.html

[S58] C++：命名空间
来源：http://hz.yongpay.top/gtbnuiofgc.html

namespace ns { int f() { return 1; } }
来源：http://hz.shuidangran.top/gtgpdgszwv.html

[S59] C++：静态断言
来源：http://hz.chenjidiqi.icu/gtsmgdwusi.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.chenjidiqi.icu/gtblrqwgfy.html

[S60] C++：遍历并删除元素
来源：http://hz.quarkkingdee.top/gtgcifufuz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yj20258.top/gtuuqosaus.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtcnzjqewp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.redwolf501.top/gteqqbuhrn.html

================================================================================
来源：http://hz.chenlongwang.top/gtoydjxsbr.html

[T01] Kotlin：Hello World
来源：http://hz.c1oappe.top/gtahkoqrfn.html

println("Hello")
来源：http://hz.guannengcc.top/gtgeyzbuxu.html

[T02] Kotlin：变量
来源：http://hz.ydzc1.top/gtgpagtjbt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhiwuduotai.top/gtlizfjffu.html

[T03] Kotlin：字符串模板
来源：http://hz.chenzaomai.com/gtubwvrava.html

"值: $b"
来源：http://hz.jianghu66.top/gtryycqrnr.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtsguydfsc.html

val n: String? = null;  n?.length
来源：http://hz.andypj.xyz/gtejhnaudb.html

[T05] Kotlin：when 表达式
来源：http://hz.wangshuangyany.cn/gtwknblmin.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhengqikj.top/gtqkobnzgs.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtwwrmppqq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.xylfe.cn/gtfdowktgo.html

[T07] Kotlin：集合过滤
来源：http://hz.jinqigufen.top/gtnidixlgn.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xinyue.icu/gtokglseyd.html

[T08] Kotlin：数据类
来源：http://hz.yuanzhike.top/gtuaihrmxu.html

data class User(val name: String, val age: Int)
来源：http://hz.gaohongyu789.top/gtqoasgcxw.html

[T09] Kotlin：扩展函数
来源：http://hz.zhijiandao.cn/gthhckqhob.html

fun String.exclaim() = this + "!"
来源：http://hz.xinyue.icu/gtabtcothz.html

[T10] Kotlin：默认参数
来源：http://hz.smart0.xyz/gtzyrauzyv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.9152youxi.cn/gtmbxdttrg.html

[T11] Kotlin：协程
来源：http://hz.xuanzx.com/gtyabdtdff.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cucudq.cn/gtugonrkfo.html

[T12] Kotlin：解构声明
来源：http://hz.daria6918.cn/gtlxvjuquw.html

val (a, b) = Pair(1, 2)
来源：http://hz.xziqi.cn/gtvaxbbvvx.html

[T13] Kotlin：只读 Map
来源：http://hz.gogol.net.cn/gtjwrxtfdo.html

val m = mapOf("a" to 1)
来源：http://hz.zhijiandao.cn/gtvyetwqfe.html

[T14] Kotlin：循环
来源：http://hz.jinqigfzy.top/gthihpxsnn.html

for (i in 1..10) println(i)
来源：http://hz.c1oappe.top/gtugdoxygx.html

[T15] Kotlin：接口
来源：http://hz.jinqigufen.top/gtfhvjjcck.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtbqsesazx.html

[T16] Swift：Hello World
来源：http://hz.quarkkingdee.top/gtkoumtvrg.html

print("Hello")
来源：http://hz.shangyingyoupin.top/gtzacyciep.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtugajmsvq.html

var a = 1;  let b = 2
来源：http://hz.chenjidiqi.icu/gtdnfebwbi.html

[T18] Swift：字符串插值
来源：http://hz.chenjidiqi.icu/gtuyjcfmyf.html

"值: \(b)"
来源：http://hz.chenzaomai.com/gtspircwvu.html

[T19] Swift：可选绑定
来源：http://hz.yj20258888.top/gtryxhxpae.html

if let n = opt { print(n) }
来源：http://hz.zhiwuduotai.top/gtndazaovb.html

[T20] Swift：数组操作
来源：http://hz.yangfankeji.com/gtrbswhqhj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.cheryme.top/gtoyfqftjc.html

[T21] Swift：遍历
来源：http://hz.redwolf501.top/gtaigkggoi.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtqgipzxmc.html

[T22] Swift：字典
来源：http://hz.pengpengdd.cyou/gtcfqdwlxc.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.andypj.xyz/gtblnrwemz.html

[T23] Swift：函数
来源：http://hz.yongpay.top/gthsdfgwek.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.tianlin.xyz/gtppfimgpi.html

[T24] Swift：闭包
来源：http://hz.zhoulong.xyz/gthxeasqor.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shzxlz.cn/gtaqsjtlgq.html

[T25] Swift：结构体
来源：http://hz.kuanghao11.cn/gtjmyvflgl.html

struct P { var x: Int }
来源：http://hz.pengpengdd.cyou/gtodvfpyow.html

[T26] Swift：类与重写
来源：http://hz.kuanghao11.cn/gtbxfxwhqt.html

class A: Base { override func f() {} }
来源：http://hz.jqgufenzy.top/gtygyqebde.html

[T27] Swift：错误处理
来源：http://hz.zhiwuduotai.top/gtyourxlqz.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gtxptlpsmf.html

[T28] Swift：枚举
来源：http://hz.zhiwuduotai.top/gtfpociclv.html

enum Color { case red, green }
来源：http://hz.feifeiyinyue.top/gtufaspjjj.html

[T29] Swift：guard 提前返回
来源：http://hz.chenjidiqi.icu/gtpwjursrj.html

guard let x = opt else { return }
来源：http://hz.ydzc1.top/gtkplcegsv.html

[T30] Swift：协议
来源：http://hz.guowangkeji.top/gtsuvyaheu.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgufenzy.top/gtumuwfhyl.html

[T31] Lua：Hello World
来源：http://hz.yj202588.top/gtcbxxqjgw.html

print("Hello")
来源：http://hz.shzxlz.cn/gtbfzialyt.html

[T32] Lua：局部变量
来源：http://hz.vqdsnc.cn/gtldmtdztl.html

local a = 1
来源：http://hz.yongpay.top/gtgliozfbd.html

[T33] Lua：表（数组）
来源：http://hz.zycfv.cn/gtnsqjubmv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.shanyushiyangtech.top/gtonhtqlzx.html

[T34] Lua：遍历表
来源：http://hz.yueranfly.top/gtppakoofu.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhiwuduotai.top/gtstubusea.html


<!-- 参考信息 -->