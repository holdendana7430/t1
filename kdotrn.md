代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.jinghuilouyu.cn/gtkcyxurwf.html

[R28] 浮点运算
来源：http://hz.jyoumei.cn/gtzjgfavsv.html

echo "scale=2; 10/3" | bc
来源：http://hz.jyoumei.cn/gtxhnvenmr.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtgbeclbuj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jqgfzy.top/gtawndplxk.html

[R30] 函数返回状态码
来源：http://hz.316326.xyz/gtnolbhfxe.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gotoacloud.top/gtiwhgkrft.html

[R31] 局部变量
来源：http://hz.shuidangran.top/gtemkmhwez.html

f() { local x=1; echo "$x"; }
来源：http://hz.smart0.xyz/gtrenvnuey.html

[R32] 参数个数校验
来源：http://hz.jinghuilouyu.cn/gtvvbtadyb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gtxrmayfsy.html

[R33] 捕获错误并提示行号
来源：http://hz.jqgufenzy.top/gtmefsvhpt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtyvsdrxnu.html

[R34] 退出时清理
来源：http://hz.yuanzhike.top/gtkowonlyr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtonkjbnpf.html

[R35] 后台执行并等待
来源：http://hz.hnqzz.top/gtlxgnhibl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shuidangran.top/gtjeaifakn.html

[R36] 并发执行多个任务
来源：http://hz.vqdsnc.cn/gtrxxishvf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtsowaajci.html

[R37] 把输出赋给变量
来源：http://hz.kuanghao11.cn/gtdluuowaf.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtvoctexoe.html

[R38] 管道串联
来源：http://hz.yuanzhike.top/gtwcrgodpu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhengqikj.top/gtuoptrixz.html

[R39] 重定向标准输出与错误
来源：http://hz.jinghuilouyu.cn/gtnpwhtgtr.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gttqxpvehu.html

[R40] 追加写日志
来源：http://hz.316326.xyz/gtvloixkwt.html

echo "log" >> out.log
来源：http://hz.nanxuanxn.top/gtlrfoilmr.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gtlvgcxgta.html

cmd >/dev/null 2>&1
来源：http://hz.cheryme.top/gtowxnoswu.html

[R42] 输入重定向
来源：http://hz.redwolf501.top/gtzudqfkve.html

wc -l < a.txt
来源：http://hz.xziqi.cn/gtawnefufq.html

[R43] 按名字查找文件
来源：http://hz.xinyue.icu/gtyilirxuq.html

find . -name "*.log" -type f
来源：http://hz.ywan-chungtsiang.top/gtrqqzewso.html

[R44] 按修改时间查找
来源：http://hz.xuetiantiany.cn/gtcnblpsiq.html

find . -mtime -7 -type f
来源：http://hz.vqdsnc.cn/gtpqaneaxz.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtkazdcqlu.html

find . -name "*.tmp" -delete
来源：http://hz.yvedp.cn/gtwrptoqrl.html

[R46] 递归替换文件内容
来源：http://hz.xuanzx.com/gtpephojqw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtkqzeohyv.html

[R47] sed 单行替换
来源：http://hz.hywenlv.cn/gtedrbzoyu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtiewkmine.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtgmymckqf.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtcgbqmldd.html

[R49] awk 带条件
来源：http://hz.gogol.net.cn/gtollnoiyf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinghuilouyu.cn/gttowbbiyw.html

[R50] awk 求和
来源：http://hz.nanxuanxn.top/gttzhasgcv.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtukekckwz.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtvshcaaoj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtazbhflnf.html

[R52] 统计行数
来源：http://hz.bjfxy.top/gtityarjvy.html

wc -l a.txt
来源：http://hz.mhx1999.top/gtiltirwwk.html

[R53] 查看文件头与实时尾
来源：http://hz.sufxvd.cn/gtcmrthpyg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shangyingyoupin.top/gtonfwqwjg.html

[R54] 比较两个文件
来源：http://hz.guowangkeji.top/gtirqmcffk.html

diff a.txt b.txt
来源：http://hz.ivvv.top/gtuqyeaxms.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtvjnqekyj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtuklavsjx.html

[R56] 远程拷贝
来源：http://hz.shzxlz.cn/gtcpfxdlbt.html

scp file user@host:/path/
来源：http://hz.guowangkeji.top/gtmilthyme.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtdyfhivju.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtgtxfmzpf.html

[R58] 下载文件
来源：http://hz.jinyuanbaomall.cn/gtomwxkmvo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gogol.net.cn/gtzxhezrvg.html

[R59] 发 POST JSON
来源：http://hz.yuanzhike.top/gtcerreavz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtvfkfmfrr.html

[R60] 只看 HTTP 状态码
来源：http://hz.feifeiyinyue.top/gtjzsuapnq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxuanxn.top/gtcnuhdgaj.html

[R61] 磁盘占用
来源：http://hz.birdmap.top/gtxskutojt.html

df -h;  du -sh *
来源：http://hz.jqgfzy.top/gtiikxntsk.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtyvfdbegb.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtnuhtnhdx.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtgxuircmi.html

free -h;  ps aux | grep nginx
来源：http://hz.dashuyun.cn/gtjhbhrdky.html

[R64] 结束进程
来源：http://hz.xylfe.cn/gtmsykjttw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ydjk.org.cn/gtouqrcjiw.html

[R65] 查看端口占用
来源：http://hz.c1oappe.top/gthzgmrofg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenzaomai.com/gtdntjeesl.html

[R66] 定时任务
来源：http://hz.ybcxt.top/gtpspfzfkq.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gtehadtfqs.html

[R67] 生成随机十六进制串
来源：http://hz.jiagoushi.top/gtcslejhnc.html

openssl rand -hex 16
来源：http://hz.chenzaomai.com/gttclyjhkq.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gtfrrhitdb.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhongyouzk.top/gtfswjroyz.html

[R69] 生成随机密码
来源：http://hz.xuanzx.com/gtozcvubyj.html

head -c 16 /dev/urandom | base64
来源：http://hz.hfpthk.cn/gtzabknrho.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gthodlkhet.html

date +%s;  date -d @1700000000
来源：http://hz.zhongyouzk.top/gtritohvxv.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtrzthvwsc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sweek.top/gtbismmteu.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtbufhzfzo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.tanke756.top/gtjpsugzzi.html

[R73] 分割大日志
来源：http://hz.bjfxy.top/gtfjquootb.html

split -l 1000 big.log part_
来源：http://hz.yonumen.top/gtrlcnmrzj.html

[R74] 批量重命名
来源：http://hz.daxiang520.top/gtlqpvdmvk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gotoacloud.top/gtsuqiiyta.html

[R75] 导出环境变量
来源：http://hz.ywan-chungtsiang.top/gtixssoyog.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtpfwcatml.html

[R76] 使用临时文件
来源：http://hz.yvedp.cn/gtxpabdwdn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtvufnotre.html

[R77] 读取用户输入
来源：http://hz.yj20258.top/gtrovshmmo.html

read -rp "请输入: " ans
来源：http://hz.jianghu66.top/gtauipfcrq.html

[R78] 交互式菜单
来源：http://hz.cucudq.cn/gthgkjaxmx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shanyushiyangkeji.top/gtkjvllztv.html

[R79] 解析命令行选项
来源：http://hz.jinghuilouyu.cn/gtljlinjin.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydjk.org.cn/gtnytgxpka.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gtfppoylqq.html

time ./run.sh
来源：http://hz.jianghu66.top/gtexaltisq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtcmyjstwp.html

S. C / C++ 专题
来源：http://hz.haohaochexian.top/gtkhkjhvvi.html

================================================================================
来源：http://hz.c1oappe.top/gtvlgwfsuu.html

[S01] C：Hello World
来源：http://hz.tianlin.xyz/gtrnjzikwk.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtacigagsf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtbfsecuwy.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtjwvkkege.html

int a = 10; printf("%d\n", a);
来源：http://hz.daria6918.cn/gttppqwurn.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gtjglereeo.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtyrvpwrsx.html

[S04] C：字符串复制
来源：http://hz.jiagoushi.top/gtehnrxmcs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.9152youxi.cn/gtmvecyzeq.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtfavsrdiy.html

strlen(s)
来源：http://hz.redwolf501.top/gtfvtwnuhd.html

[S06] C：字符串比较
来源：http://hz.yongpay.top/gtxiyodrvj.html

strcmp(a, b) == 0
来源：http://hz.tanke756.top/gtvkajfwch.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtekivbsyt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shuidangran.top/gtmbidgkfy.html

[S08] C：动态内存分配与释放
来源：http://hz.hnqzz.top/gtvgvazmah.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sweek.top/gtrnwgotvp.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtgjgvozrc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtbfntjthc.html

[S10] C：指针与解引用
来源：http://hz.daxiang520.top/gtppkvrrqf.html

int *p = &a;  *p = 5;
来源：http://hz.ivvv.top/gtfdytvfus.html

[S11] C：逐行读文件
来源：http://hz.daxiang520.top/gtmorcnbii.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinghuilouyu.cn/gtexdylyxo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gaohongyu789.top/gtidyrmggf.html

fclose(f);
来源：http://hz.zycfv.cn/gtbhweehhp.html

[S12] C：写文件
来源：http://hz.sweek.top/gtxhnghdfz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daria6918.cn/gthbvrzwmn.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtyznikbhn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxuanxn.top/gtgjncskfy.html

[S14] C：枚举
来源：http://hz.redwolf501.top/gtzssibasr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtrkqzidlb.html

[S15] C：类型转换
来源：http://hz.zdqjudy.top/gtqgvzgspu.html

(double) a / b
来源：http://hz.aizwys.cn/gtwypctrxe.html

[S16] C：位操作置位
来源：http://hz.ivvv.top/gtenvabmpu.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtjqkdqwtt.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtfbhgorgk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhaomingkeji.xyz/gtczolilcb.html

[S18] C：命令行参数
来源：http://hz.tianlin.xyz/gtyaudnpfz.html

int main(int argc, char **argv)
来源：http://hz.yongpay.top/gtrmbfhvfh.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtahkkilyw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtmfegjswv.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtvjmmwrxa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hnqzz.top/gtteutevtf.html

[S21] C：字符类别判断
来源：http://hz.xinyue.icu/gtmvzvcfzo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jianghu66.top/gtbxzncpca.html

[S22] C：字符串转数字
来源：http://hz.mhx1999.top/gtpgcnpygd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.wangdashe.top/gtxzjwmdrh.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtaoftfsne.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinyuanbaomall.cn/gtlufneqcy.html

[S24] C：获取本地时间
来源：http://hz.andypj.xyz/gtalsurddt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtmvztmctj.html

[S25] C：内存拷贝
来源：http://hz.haohaochexian.top/gtbtkfgaqu.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtkdvyifpx.html

[S26] C：内存清零
来源：http://hz.yongpay.top/gtotuugkfl.html

memset(a, 0, sizeof a);
来源：http://hz.sysykeji.top/gtspklvhqk.html

[S27] C：定义常量
来源：http://hz.dashuyun.cn/gtovanxnhd.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtpiqssdwx.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtzcupakgr.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtuemldiec.html

[S29] C：变参函数
来源：http://hz.hammf.cn/gtwgkyeepd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.snrcjt.cn/gtawtesxwy.html

[S30] C：头文件保护
来源：http://hz.birdmap.top/gtbobxtvbi.html

#ifndef X_H
来源：http://hz.cashguo.top/gtabjtahlf.html

#define X_H
来源：http://hz.sysykeji.top/gtdzjbkcrm.html

#endif
来源：http://hz.sxryk.cn/gturcaiasd.html

[S31] C++：Hello World
来源：http://hz.pycfn.com/gtjtwlzqlm.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtowilivvo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtqvcpaczg.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtlqdnvwvv.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gtxqxbytkk.html

[S33] C++：vector 增删
来源：http://hz.gzhubu.top/gtfrpndakj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zycfv.cn/gtrqhdcgym.html

[S34] C++：遍历 vector
来源：http://hz.guannengcc.top/gtvpfnuqzg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.wangshuangyany.cn/gtuibfspwa.html

[S35] C++：map
来源：http://hz.xziqi.cn/gtqulqbxra.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shzxlz.cn/gtqkoadjpg.html

[S36] C++：unordered_map
来源：http://hz.c1oappe.top/gtnwmzszpc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtwtpztlvt.html

[S37] C++：set
来源：http://hz.shuidangran.top/gtnhtevsew.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtqhznfodu.html

[S38] C++：排序
来源：http://hz.zhiwuduotai.top/gtlzltjlvt.html

std::sort(v.begin(), v.end());
来源：http://hz.gzhubu.top/gtehtjwbgc.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gtunersnnl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.smart0.xyz/gtsaqautwf.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtnagfxpih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hammf.cn/gtwbbzzzab.html

[S41] C++：类与构造函数
来源：http://hz.pycfn.com/gtchteipps.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gtiiihcwio.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtpptmxpyz.html

class B : public Base { public: void f() override {} };
来源：http://hz.cqqwz.cn/gtkpkybpuw.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtlhimmudb.html

auto p = std::make_unique<int>(5);
来源：http://hz.yongpay.top/gtoldwinnu.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtckblpoyx.html

void inc(int &x) { ++x; }
来源：http://hz.cdnleiting.top/gtghznivgz.html

[S45] C++：lambda
来源：http://hz.gzhubu.top/gtsxvuczch.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.0kj1m.cn/gtikjdunjs.html

[S46] C++：函数模板
来源：http://hz.xingfuxueyuan.xyz/gtxzbfucmv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258888.top/gtfzcbgpvv.html

[S47] C++：结构化绑定遍历
来源：http://hz.9152youxi.cn/gtrktdwyje.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj20258888.top/gtkwtgsqvd.html

[S48] C++：逐行读文件
来源：http://hz.52xcode.cn/gtiwkgpupo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhiwuduotai.top/gtbxnbkyyl.html

while (std::getline(in, line)) { }
来源：http://hz.zhoulong.xyz/gtrbxhlppe.html

[S49] C++：写文件
来源：http://hz.snrcjt.cn/gtjnvhvxau.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj20258.top/gthzlzooul.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtlyxsdkxo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtomdxwilz.html

[S51] C++：显式类型转换
来源：http://hz.tianlin.xyz/gtsphexjgj.html

static_cast<double>(a) / b
来源：http://hz.hammf.cn/gtyjwoikmm.html

[S52] C++：const 与 noexcept
来源：http://hz.hammf.cn/gtfrehzuxy.html

int size() const noexcept { return n_; }
来源：http://hz.gotoacloud.top/gtudxiozrh.html

[S53] C++：移动语义
来源：http://hz.zycfv.cn/gtzrweltkv.html

std::vector<int> w = std::move(v);
来源：http://hz.ybcxt.top/gtiykuirjp.html

[S54] C++：异常处理
来源：http://hz.ivvv.top/gtzmbmvayo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.redwolf501.top/gtulqsdiun.html

[S55] C++：结构化绑定
来源：http://hz.tanke756.top/gtpxqihzhc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.fengsongda.top/gtaaddfspf.html

[S56] C++：optional
来源：http://hz.kuanghao11.cn/gtyuvjggnn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yongpay.top/gtvosqupjd.html

[S57] C++：编译期常量
来源：http://hz.zhongyouzk.top/gtyjvekkyt.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtnvfotrfg.html

[S58] C++：命名空间
来源：http://hz.birdmap.top/gtnpmlahme.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtvdkvujzb.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtnuuepxls.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.mhx1999.top/gtymfdtbyu.html

[S60] C++：遍历并删除元素
来源：http://hz.cqqwz.cn/gttmocxhuu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.havefunace.top/gtjhmoyslj.html

================================================================================
来源：http://hz.jianghu66.top/gtijszdpsf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.xinyue.icu/gtcwtgxygh.html

================================================================================
来源：http://hz.daria6918.cn/gtrwoyeejp.html

[T01] Kotlin：Hello World
来源：http://hz.nanxuanxn.top/gteahxiyqo.html

println("Hello")
来源：http://hz.feifeiyinyue.top/gtmswtmolb.html

[T02] Kotlin：变量
来源：http://hz.gogol.net.cn/gtfdvdrdwl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yueranfly.top/gtxiaqkdpf.html

[T03] Kotlin：字符串模板
来源：http://hz.zhongyouzk.top/gtjvzzmgtj.html

"值: $b"
来源：http://hz.yj20258.top/gtfpkgljls.html

[T04] Kotlin：空安全
来源：http://hz.daria6918.cn/gtkuzjnzwf.html

val n: String? = null;  n?.length
来源：http://hz.yueranfly.top/gtbpwfozyn.html

[T05] Kotlin：when 表达式
来源：http://hz.dianchejie.cn/gtluvkiogd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hnqzz.top/gtpyyzwebx.html

[T06] Kotlin：集合映射
来源：http://hz.wangshuangyany.cn/gtiumdrucm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.tian-w.cn/gtjiyhaqso.html

[T07] Kotlin：集合过滤
来源：http://hz.ydzc1.top/gtwxvfbina.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.svipenyu.cn/gthriswwcx.html

[T08] Kotlin：数据类
来源：http://hz.cheryme.top/gtldnrqxjm.html

data class User(val name: String, val age: Int)
来源：http://hz.cheryme.top/gtecatcuea.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtymfbylkp.html

fun String.exclaim() = this + "!"
来源：http://hz.jinyuanbaomall.cn/gtnlcojfuz.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtagdrvyac.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yuanzhike.top/gtepekzynv.html

[T11] Kotlin：协程
来源：http://hz.daria6918.cn/gtaluqvliy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenlongwang.top/gteygwebgf.html

[T12] Kotlin：解构声明
来源：http://hz.tianlin.xyz/gtiurdghnc.html

val (a, b) = Pair(1, 2)
来源：http://hz.jinqigfzy.top/gtqgxjdctk.html

[T13] Kotlin：只读 Map
来源：http://hz.yanxiufei.cn/gtfloyxlqp.html

val m = mapOf("a" to 1)
来源：http://hz.hnxiangtu.top/gtwdribhuf.html

[T14] Kotlin：循环
来源：http://hz.ydzc1.top/gtlnakythc.html

for (i in 1..10) println(i)
来源：http://hz.shangyingyoupin.top/gtcldebbrb.html

[T15] Kotlin：接口
来源：http://hz.jinqigfzy.top/gtyiozzfkr.html

interface Shape { fun area(): Double }
来源：http://hz.hfpthk.cn/gtfmqqyugy.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtofphllwj.html

print("Hello")
来源：http://hz.quarkkingdee.top/gtugmlawwn.html

[T17] Swift：变量与常量
来源：http://hz.xziqi.cn/gtfntoasda.html

var a = 1;  let b = 2
来源：http://hz.hongshengwenyu.top/gtdzgiklbd.html

[T18] Swift：字符串插值
来源：http://hz.ehwqpu.com/gtnaibhwsl.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtcrrdicam.html

[T19] Swift：可选绑定
来源：http://hz.yonumen.top/gtarwwvpjf.html

if let n = opt { print(n) }
来源：http://hz.sweek.top/gtwncbzrha.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gtrouiepiz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.ehwqpu.com/gtwrxhaytz.html

[T21] Swift：遍历
来源：http://hz.yongpay.top/gtbgclizfu.html

for x in a { print(x) }
来源：http://hz.pycfn.com/gtlkkxbplf.html

[T22] Swift：字典
来源：http://hz.ywan-chungtsiang.top/gtuykhiodo.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.aizwys.cn/gtetvuyjna.html

[T23] Swift：函数
来源：http://hz.yvedp.cn/gtbmefbxpv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.316326.xyz/gttleepiki.html

[T24] Swift：闭包
来源：http://hz.tian-w.cn/gtklqifzod.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.zhaomingkeji.xyz/gtwbbvrerz.html

[T25] Swift：结构体
来源：http://hz.jinyuanbaomall.cn/gtpnfshvzj.html

struct P { var x: Int }
来源：http://hz.yvedp.cn/gtitqloivl.html

[T26] Swift：类与重写
来源：http://hz.smart0.xyz/gtydnwvpnq.html

class A: Base { override func f() {} }
来源：http://hz.nanxuanxn.top/gtdmzchqny.html

[T27] Swift：错误处理
来源：http://hz.dianchejie.cn/gtgwgzvpoc.html

do { try f() } catch { print(error) }
来源：http://hz.svipenyu.cn/gtnelgbkue.html

[T28] Swift：枚举
来源：http://hz.yangfankeji.com/gtzfpcmjnf.html

enum Color { case red, green }
来源：http://hz.xinyue.icu/gtvgeklogw.html

[T29] Swift：guard 提前返回
来源：http://hz.bjfxy.top/gtlnqwngoh.html

guard let x = opt else { return }
来源：http://hz.ywan-chungtsiang.top/gtmdqesdol.html

[T30] Swift：协议
来源：http://hz.hywenlv.cn/gtwzderwah.html

protocol Shape { func area() -> Double }
来源：http://hz.316326.xyz/gtbosfnkxn.html


<!-- 参考信息 -->