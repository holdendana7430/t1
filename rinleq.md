代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mqdacyzk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ehprdbtd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2csaigavy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2thlawksl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2usortrlk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2brcpkoym.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dyegpnci.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2urvuatcu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2pwgnlhar.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mrhrquta.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dbbrfyim.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kuqprizd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsfbljiz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rxgiyiuu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2iaomteqk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rsgaowkb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dxhsxjye.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hsowvrpu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gzxicsma.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2gayldabo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kdetqggw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mvbwybtk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vjzksaey.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jcwxneny.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yifobgjf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2uzctukrn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qybyyzue.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uatggtab.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2accohafd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2llocvrph.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2fzsgocae.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2aulnwfri.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yhlyinkk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2moaflscy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lspquubd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2kfhvymwh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2husrhaal.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ntqvlist.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vamjrypd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cwaftrzw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sjwkwexw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2aqnfqtxv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2lgebspxe.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2jfqgtzkr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tbaicwek.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2iphgucjg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jdyumfkt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2mzyzuzlv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2awmadkel.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jhbtbnqu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vyumpcma.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vafmruxb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mgvfbysk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqjeeyrr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2opsdcbtp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hejyphem.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lqspvqhf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kcwoxxry.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2rhtctahj.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2qfifmwaq.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nhyfvnwz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gfdlkfva.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pjskuxqc.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kcgxyozy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bpaimagd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ejoebqoi.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2vbaafkpn.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xhkozjce.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ioxfawus.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hqrbaras.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2eadcmczh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nhlanqtj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ydebzvbe.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2esyajhlg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2odxgxzil.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dygkeccq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2apkcuinv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qovnnbjo.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ceidfyvg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dmdysztq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2qfirxvkx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2nfuiknqs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ptdcufwv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2lttsibas.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2imqgtbbo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ukursjif.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2dvrozrxm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ictltpmq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2iuergncq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2qmnxmodn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mhhwbnuc.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2effounrb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2cjzggpbx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2omlgkmyz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vutsxduc.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2oxneywyj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wjdvmsvj.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pxnlhadd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xiwtqqhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxalfrtv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pgopshkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cebvxwbc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2licjoczb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sxhtkyhs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydcpanfd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ggveolpg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdvzsae.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ocwqjlnm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cgkwylrd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ourdyrcm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2psxbrqfw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wybfnocn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kscogzrd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2xbnaluxk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wiwjtvkf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kgnwsioj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ymeatxgh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lavtkhct.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2spmvewkk.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2gbkmtsli.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2xqygaklw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rgadhocy.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hpgjzazd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jyioqjqh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2djolcrle.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qurzidgo.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qgxekiop.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ajufnaiu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2umqpyelz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2thfeeqtz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zpgwjqny.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hgwhvwdr.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tcvqonvf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2qjhulubc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2vabngqgz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2yskrmewh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2paidslbj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ssslqwxn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2knhkwvym.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eialqgdg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2tksfzjqp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ztleparb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2wygdcnkj.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2bgbvryko.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ysvmhmol.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2cuaxcgte.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2byzbyfoc.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2nbmclydf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2vcstercg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bmpodwqq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ndkdxrdu.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2kpilwhoz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2nmyocfgt.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2snebpipq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ovsbzfzs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2pinevcqb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2lkgftzpg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2eatcqjcm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qsorpmes.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2oekhmcxl.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2rzopxhke.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2btedfwwy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2fpgrlste.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2cnnfxquz.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2vwfsmape.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2iksjfjdz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ulvnvqpx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oayqmqwn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2iecaypid.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2mcmnrzaf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wcllsbgs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2fdcxiumg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ltgbhvdo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2obdyxfgt.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2iyfyjnda.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2tjislcve.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2cmjugqkn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kvcsfizg.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2fppbzvzk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nmzrjplu.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ogxodgya.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hgphhtsb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2mamgdccj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2mwetzfak.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2zooqbpms.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2clyicgkw.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cpevqybe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2yxsrwaiq.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnpenewe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ixvezpzy.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2pmduazjz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2vrwvceae.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2xkqpiscb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cvtsijue.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xbzmksyy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbzwhyji.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2klvjywll.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2doekpxbc.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2smfrtxwy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pckrjbbl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2ddvkwuhh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2tojokocv.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tzcpzfvh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2wezhebfx.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2sxyefkfj.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2tadjyhef.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2usdmysls.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rmcpibva.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gvmlwmpt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2gxmnucpf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2vgyveipb.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2xtgjkhcj.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2junsxrqi.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2oqwpdkak.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2njywqyfu.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2rftpcque.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqzrvvt.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2sljiikua.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2chodycvo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ogfucmlo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyaxlomm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2gxmfgnmq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2byiotmpq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2utsvbfaz.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfthfxr.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2rrosfrth.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2vosrpzut.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jzsejxfs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fyzhzxlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdqsvynr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2sehkzixt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hadguakz.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2iigcszsd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oaebtvak.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2avzvbsvo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ylwamkji.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ulsgvtuw.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ileoekmh.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2sftefkrx.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2cptolbcm.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2avgdwpbc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2vrlvvxog.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2smuulplh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ljlykefe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2binopput.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eliblrth.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2xmczowpg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2rroiqvvh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkgprsmv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2rezicvtk.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2gmisyiif.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2qtvanmaf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2apakqvyw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2mfxybzwc.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2yifodygp.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2quaypxvg.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2tvoqhvqb.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sknujawk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2vkuwpklq.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2obteujmo.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2opfhnexa.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2bnnerbfl.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhhuesxg.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xyhgwoqv.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2fukdwbfj.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2ypugruqj.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mblogvfm.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ujhxncpi.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2styepsfy.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2pgbablyd.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2aswlyucw.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ldepmfkj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2frfgbqio.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vakcbanm.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2kkbrsxda.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2uhczjjcg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2kwazjxzy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vflakhor.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2pdygjpfd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zzibuasf.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2nxndnsip.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2rdgvxnde.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2lzyvwujj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2svneocrj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yiecwqdv.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2arhzgwhb.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2nxoyoivv.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2hnbpssjo.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2utiptofr.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2nmsxgafy.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2bowflocw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gkbpteoh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2laccrlqu.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2mytvitgr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2bgchaoyr.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2pimzwtwt.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2bssrlvpj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2pnlxoilt.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dlpcxbcj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2wouqkrwq.html


<!-- 参考信息 -->