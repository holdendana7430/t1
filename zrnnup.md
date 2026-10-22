代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2iizutdco.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mifqoanm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kypnhtfc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rwmlxjby.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2unteudgn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2xnxgyeoz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2rrjimffj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2crployjs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2uecksecw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pspgsmna.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ilqoswwa.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hgnwpqbf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kbsgmnfl.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sjxbleer.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yhjogsos.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2notyyvsv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2lmsdozjn.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kmixobnc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lipyrthp.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqatdxty.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2osrwurne.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2abaiwzbr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jyiwjjay.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tdoqravr.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kpkenikt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2hmgtkoex.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2rndezlrr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cbzryknv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lrrteiek.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2tmoqfzts.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2natrynml.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dbutwnvg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2poiyztyd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ttccjduy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xfnlxdgl.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2trzmjpma.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zeszvsak.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2clnmcrve.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tyxpdetu.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rrrmvscu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2lhtjyrue.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gijmhqba.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uchqgmfy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ovksbpfl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hjyxtlfv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wpmersnw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2onizxuqi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2zvvtjsrd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2addsixkb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngtwuncb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2acrxbamv.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bozddbcc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2inhryybe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gsaakwhq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jqldccjb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2waczpqrx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wdoqgzqw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvnqoysp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2olyaqxry.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pzqhdtkx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lzywhueq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rrtftlli.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2oaycgmnr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2oivqgxeo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2obknhtlv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2vshnipfo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hmpetaul.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2utqbikqv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qepcvbbn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nvttwawx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2zhszjthn.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2sphrrbai.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pbilylwc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2gjqtzsoj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pgqvsguz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dswxyflf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2ffugrmbs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2tixbgrna.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kqxtwquk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2sbkarfey.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2azxyvqpo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2vjyrxgri.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdhuwnbo.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xrqicbib.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ffuouevj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dihxsgyx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2hluyqgfh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2jkxyyuwz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vlqhrfle.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2hfxflxai.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2xemvnkys.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2hlbrzsik.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zrpnizea.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2yyoyqoqi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ywhnbkwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkbdbyht.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qxmwgptp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfyflfph.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2bgbcnqmm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2acytfdyp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mpohchqu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bvicpidz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xcrbfhbg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ntrxuxlr.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2lbvezfpu.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2jhkzldsw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mckcsanp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nzxurzii.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hempkrbx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2axurftlz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2xzaelqhf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vjwtbiua.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2uncltqgq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wqyrgfmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2pfchewwn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2bzqercxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jopebzsl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2boghnblk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2teiwliva.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vvttwkpi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2dbvzqgve.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2tftqjggw.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fqwrmbrf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2zzaqgtrr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ixlfgulj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jotsvqgw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2trkoxrwl.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2jzpgspbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2svcqcctf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2gyedtgts.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2taueibje.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2bvbgznex.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jevcbycw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lguyynnz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2evnqvvrj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdoqynlm.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2hovnvwhu.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2bhjqbmwp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2hurdwtbv.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2indvsxmt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sotsegsw.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2qitlvckh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2oewjsady.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2cqayqemt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2khpqttsa.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ebqnxlgh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2toemtgpi.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gygsyiug.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2prmulgxu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2alppgxwc.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vqlxhigs.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zxatuwyn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2rqphyjch.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2iyvuyfll.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ncgpmesb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2bqveyyrx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ftrkrlct.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2tewrywbd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2kxbqjxpn.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wpywbply.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2xfevfdrv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2hujeofgx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wdavekju.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ytmfyffo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2iqsluczp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfmwxwdo.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2bpvogpds.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2gikmttnp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gfwllkwh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mnjkszis.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2hcmcwvvl.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cagvjmua.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pdtwkqop.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ltuxtrsa.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2engofona.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cvbchfgf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2vzdiovea.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2wxlkuhoj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ewogipox.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2kndmzujf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2xtschcjq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2saxgisxe.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2ermrwndx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uhduvrdy.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2arnrxelh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2gdtermcc.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2kkobxene.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2ztftmldi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ohwtcbit.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rtskzmyp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2yagvaoib.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2bardvjab.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kwqlntur.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2pgsqxlrs.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2zofofgpu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybedwzge.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2mnlecrgf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsxxngsf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lzzjpdsq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2celzjkkn.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2waivozub.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2acoxlabz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2kvotjdcz.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2cxowdbma.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ourrqkup.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2exlnasww.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uaqjsqkc.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2jjkhsexl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2csvhvfnv.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2bxigzkpp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2hqqcemci.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2kvrhiyie.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ajhopelh.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jkxdnykj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lklzmezo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2pqtnfpbr.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojyihrxi.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2nwkqnahz.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cdfrbucy.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2sqwawfrr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2onetuojv.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hfcnkvlc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ufqnpqvg.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iwblwhhn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2neikutyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmbyrgyd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2yyxavokj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtemgpzx.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zojogaqx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bsaggedb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2rsywjnmt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2uwkmfbop.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kqsiiknk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2connhypu.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2etqmfegs.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2vlubufwa.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gdhloewy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2lfjsaabp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2sbqgszbc.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbcgbxs.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wqunrygd.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2howfcqne.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2iibkhfax.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2skiucyer.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2uiqhqsjt.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2qyxcdzxf.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2aiwhjzvz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2lzvggmuf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dnkdfsoh.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2swsiiqjz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2mzautcyz.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zabslbsa.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2qgffvqop.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aytmtbhr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2gexombhr.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2yyoibdiq.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2biunuifo.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ygwtrmlz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vfbvkcel.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2lvsaqkbm.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2nkekijan.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2iopumatz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2uyhkftyw.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2vbrqjdbb.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2odqcnwlt.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2itdywotc.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2qzsvnjqj.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2drurerpc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2gxtgyntl.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ymkotgxh.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vqwxvwnn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uvlhoqge.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2jhkomcsu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2inhgyfxg.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2usymplhz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2omkopkjt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2yhmrkswg.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2gbbtgmme.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2kqbhfmqg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2fkupuazu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vaoduvwl.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2iwwusdyg.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2azeprfkk.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uneehdrm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ohatewjv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2tbghwzde.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2iqzuchjt.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rumnwykg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2czietcxr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rqwnntcl.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcgrqnti.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2hthjioig.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gdmhwgef.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2xppssgsh.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xotowpzs.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2rvdjgiav.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zjhfjwht.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2pispyxlr.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2osrrrgvp.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2kzfuudmg.html


<!-- 参考信息 -->