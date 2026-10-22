代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2viorearg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kxuiwadt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2clqsmddt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mzwktiln.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mzmyqktu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2xixmsgdk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2twhxrcab.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2xovixixv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2krzmtinx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qzkgavrr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ngvnxqor.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2otajdhcm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2kkngvaiq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2wwomxvuq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xmftgpel.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2egietdie.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hfpppfje.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2naghjjls.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xwmtynnv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2lvfyilgv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2encvpvhh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nmtzkvfg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykzwptmo.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xerxkzho.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zzpgywri.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2dlxlzbry.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2viomymku.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2iitwkbkn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hdsrkypi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hjxhghph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rbwcnpro.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2avhqescy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bjtupjpy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2poyaefiu.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uyiyklgc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2anngkthv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bgacdqqq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ucvjmoge.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2juvdmcfp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2epunbder.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2fvlepexw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hmbtvaec.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xkumzfoo.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2zjfjgqyo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dfchkang.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dotwqxst.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2oawtvjna.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2gqahfbwm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xbvextje.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wwqlhzik.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hyytzfoy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2tgicmqxl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2aipbniso.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhcllufy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2iewwkjoc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zapuqeip.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qcvrsrvm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2reafitmh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bdsrkhnh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jooxzruj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2gdycccqp.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2asonpgwb.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2lcmanxwk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fuaiqqaf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gggexmoa.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2bpwqzbpz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2gtszivvu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2twdwhnjz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fcgszpbp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gzhxkcci.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2corojrdw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rnswzoht.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2jjnolqla.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2uedzlufg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fynvszkj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2onyqzizw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2hlavycid.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hhchdeva.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2hjcpfgep.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bwsguqqi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ykfiqhss.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2lvmzierm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lmwcrell.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2lhsuwofj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2xffgjwef.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2fvlavpgc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2jcuujmvp.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2iathglcr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zisqxrup.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzigmpsr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bulrlsln.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2oifgwrfh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2qqrgcysg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vbbriqnp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2mwawknyo.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2gelwhdoj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zxnprqdy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vczsmhzu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jfmgyxtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcdluohy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2nfcdtdxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dmwvmffk.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ujuzylql.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2kbauqflm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2osyajllc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iqggmkjy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2kcncyura.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2nchyptav.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ucdbrlua.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2clpihobi.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jqhostzq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uotxllyr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkettzw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fzqbqnbi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ghlnxpng.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kspuaquf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2asyfmbxy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2kjeidxfi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2igncdqnu.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2xuwlycwh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2yxbcnukt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2kbuuneyu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zupwtumg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yqlkxjgd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gmtjtnlb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rtahaeqs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2bxyytcgi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2xcnkgxkz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2nqknaaag.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2rjimhqvf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2guflqmaq.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iipkcocl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2swtuyflg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xbyuhuid.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2trxjcqmc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2fblilkpj.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gpemqkwp.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fkbkfpun.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hpvdycfk.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2xiarokhe.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2thbodbll.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fuizagof.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2defopzhm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2jsecwfvr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bktrdlhd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2upucxtwq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2khwwxbhd.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2rrkqinpq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2yfkcrjit.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2utvtcmvm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2zknlzoth.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ibznpmjf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rlsuehuf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lwyxxdba.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qnwqglki.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2jqmjucwj.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2lvkqgcet.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2aqjjhbnl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nwyusrxv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2ikyptlmc.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2wxcszojr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2vgviqqud.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2dccdplqy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2wcbbidxv.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2julvlaey.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2jlkfeqge.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2wndlixtt.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tbskiuvg.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2ymtcopro.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2zehqqzds.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xxicezko.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2meslivmk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2nlrrmddh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rvpkhosv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pvuihqhf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2oyupbdfh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2unbgfhsh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2djfwvjar.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2nkozjlbs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hbmtpzki.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2zwmmcjep.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2womjbvkx.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2jjgmsjtp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ddcpqorj.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2emkkftff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2iaoddrzb.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fbroycod.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xaljvgcz.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2bgxfgakd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2izrefdbv.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2zqlsdajz.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2xuerbkhv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2vteflwwm.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2krboknin.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2dpurerpe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2smwykisk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qehqjdgp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2brglmxmw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dadaolyt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pshovoqt.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2fjcsncrv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbwghpfs.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdigygyq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2smuuvtxb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jqfopxzj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2cikjsgik.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ojwqkaya.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ecncqdlo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wlxphggl.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2hddfsqfv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2rynqlufr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2mosixsmp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zivjtdxk.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2rxscmgve.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2htoscgak.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2fsjtddve.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2vdcioshe.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2yhqddbuz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2etlgzaaf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ohqokyqx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2opclhlvk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2cezqpphx.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gbpylpht.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2otxtzhab.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2vfolehay.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pfqasgjc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2unuehhld.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2diphozmp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2yteezkhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddwxikoo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2rksjsemp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taooazxy.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mwdvqbyb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qclpncwh.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2qkmnnbhr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2bsrguphh.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2vvuspyvv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2nmjhcojq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xpzdfwsb.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2fhosumoy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2suenyjql.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2tdzyxjis.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tenpdzir.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2kupeelnl.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mtmdrahj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2wuxtrrpp.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2jvzuxduq.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2obzodrwx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhvklzsx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2gpmislby.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ewcnksxi.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ytuvjlyl.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2edrnybtf.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2pmqhkiwt.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2pleesxqn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sseozwil.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2gsoqoray.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmwwlfj.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2kpnysfek.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2fzxlkjkf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2oddlukxc.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2zlofsgjv.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zlolfrxi.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qlihgamt.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2mllsapyc.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2dzwuitlg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2yxmkwtwt.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2nwycmgob.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2janicdcb.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2eslefmio.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2vcsfpdyv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2eoafcewl.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rsseeouc.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2albhsopn.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2mgcluial.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2odlfzfaw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2ihisqrnl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2uxbgtawb.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2zfwrtdgx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnanjgzd.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2csrpjhfq.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2hhebzqdf.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ycersglw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2weldykjg.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2nhzkxfzv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2khibsebn.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ypjaubpx.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2dhwwhjpe.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xfvyluju.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2mmhzdnbg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ypepkqzo.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2cpduzitb.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tnypmrgm.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cylfjuwn.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2spyehbdd.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2zybkczcr.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fpqaqhzi.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2ntufmhnk.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2qcgoxlax.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2yngvhqqe.html


<!-- 参考信息 -->